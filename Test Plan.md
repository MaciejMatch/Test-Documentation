# Test Plan - Demoblaze E-commerce Store

## Document Information
- **Project Name:** Demoblaze E-commerce Testing
- **Document Version:** 1.0
- **Date:** January 2026
- **Prepared By:** Maciej Miszewski, QA Tester
- **Status:** Approved

---

## 1. Introduction

### 1.1 Purpose
This document outlines the comprehensive test plan for manual testing of the Demoblaze demo e-commerce application. It defines the testing scope, approach, resources, schedule, and deliverables.

### 1.2 Project Overview
**Application:** Demoblaze E-commerce Demo Store  
**URL:** https://www.demoblaze.com  
**Type:** Web Application  
**Purpose:** Educational demo for learning and testing

### 1.3 Document Audience
- QA Team
- Project Stakeholders
- Development Team
- Project Managers

---

## 2. Test Scope

### 2.1 Features In Scope

#### User Management Module
- ✅ User Registration
- ✅ User Login
- ✅ User Logout
- ✅ Session Management

#### Product Management Module
- ✅ Product Browsing
- ✅ Category Filtering (Phones, Laptops, Monitors)
- ✅ Product Details View
- ✅ Product Pagination

#### Shopping Cart Module
- ✅ Add Product to Cart
- ✅ View Cart Contents
- ✅ Remove Product from Cart
- ✅ Cart Total Calculation

#### Checkout Module
- ✅ Place Order Functionality
- ✅ Order Form Validation
- ✅ Order Confirmation
- ✅ Purchase Completion

### 2.2 Features Out of Scope
- ❌ Payment Gateway Integration (not implemented in demo)
- ❌ Email Notifications
- ❌ Admin Panel Testing
- ❌ Backend API Testing (covered in separate project)
- ❌ Performance Testing
- ❌ Security Testing
- ❌ Mobile App Testing (web only)
- ❌ Accessibility Testing (WCAG compliance)

---

## 3. Test Strategy

### 3.1 Test Approach
**Testing Type:** Manual Functional Testing  
**Testing Methodology:** Black-box Testing  
**Testing Philosophy:** Risk-based testing focusing on critical user journeys

### 3.2 Test Levels
- **System Testing:** Complete application testing in integrated environment
- **Integration Testing:** Testing interaction between modules (cart + checkout)
- **User Acceptance Testing (UAT):** Validating against business requirements

### 3.3 Test Types

#### Functional Testing
- Feature functionality validation
- Business logic verification
- User workflow testing

#### UI Testing
- Layout and design consistency
- Button and link functionality
- Modal window behavior

#### Validation Testing
- Form field validation
- Input data validation
- Error message verification

#### Compatibility Testing (Limited Scope)
- Browser: Chrome 120+, Firefox 121+
- OS: Windows 11, macOS Sonoma
- Resolution: 1920x1080, 1366x768

---

## 4. Test Environment

### 4.1 Application Under Test
- **Application Name:** Demoblaze
- **URL:** https://www.demoblaze.com
- **Environment Type:** Production Demo
- **Database:** Not accessible (demo environment)

### 4.2 Test Infrastructure
| Component | Specification |
|-----------|--------------|
| **Operating System** | Windows 11 Pro, macOS Sonoma 14.2 |
| **Browsers** | Chrome 120.0+, Firefox 121.0+ |
| **Screen Resolution** | 1920x1080 (primary), 1366x768 (secondary) |
| **Internet Connection** | Stable broadband (50+ Mbps) |
| **Testing Tools** | Manual testing, Browser DevTools |

### 4.3 Test Data
- Test usernames: QAtest_user001, QAtest_user002, etc.
- Test passwords: Test@12345
- Sample credit card: 1234567812345678
- Test addresses: Various US addresses

---

## 5. Test Schedule

| Phase | Duration | Start Date | End Date | Status |
|-------|----------|-----------|----------|--------|
| **Test Planning** | 1 day | Jan 15, 2026 | Jan 15, 2026 | ✅ Complete |
| **Test Case Design** | 2 days | Jan 16, 2026 | Jan 17, 2026 | ✅ Complete |
| **Test Environment Setup** | 0.5 day | Jan 18, 2026 | Jan 18, 2026 | ✅ Complete |
| **Test Execution** | 3 days | Jan 19, 2026 | Jan 21, 2026 | ✅ Complete |
| **Bug Reporting** | 1 day | Jan 22, 2026 | Jan 22, 2026 | ✅ Complete |
| **Retesting** | 1 day | Jan 23, 2026 | Jan 23, 2026 | ✅ Complete |
| **Test Closure** | 0.5 day | Jan 24, 2026 | Jan 24, 2026 | ✅ Complete |
| **Total Duration** | **9 days** | Jan 15, 2026 | Jan 24, 2026 | ✅ Complete |

---

## 6. Resources

### 6.1 Human Resources
| Role | Name | Responsibility | Allocation |
|------|------|----------------|------------|
| **QA Lead** | Maciej Miszewski | Test planning, execution, reporting | 100% |
| **QA Tester** | Maciej Miszewski | Test case design, test execution | 100% |

### 6.2 Tools & Software
- **Browser:** Chrome, Firefox (latest versions)
- **Documentation:** Markdown, GitHub
- **Bug Tracking:** GitHub Issues (for examples)
- **Screen Capture:** Built-in OS tools
- **Version Control:** Git/GitHub

---

## 7. Entry and Exit Criteria

### 7.1 Entry Criteria
✅ Test plan reviewed and approved  
✅ Test environment is accessible and stable  
✅ Test cases designed and reviewed  
✅ Test data prepared  
✅ Application URL is accessible  

### 7.2 Exit Criteria
✅ All planned test cases executed  
✅ 100% of critical test cases passed  
✅ No critical or high-severity bugs open  
✅ Test summary report completed  
✅ Test artifacts documented and stored  
✅ Stakeholder sign-off received  

---

## 8. Test Deliverables

### 8.1 Before Testing
- ✅ Test Plan (this document)
- ✅ Test Strategy
- ✅ Test Case Specifications

### 8.2 During Testing
- ✅ Test Execution Reports
- ✅ Bug Reports
- ✅ Daily Status Updates

### 8.3 After Testing
- ✅ Test Summary Report
- ✅ Test Metrics and KPIs
- ✅ Lessons Learned Document

---

## 9. Risk Management

### 9.1 Identified Risks

| Risk ID | Risk Description | Probability | Impact | Mitigation Strategy |
|---------|-----------------|-------------|--------|---------------------|
| R-001 | Application downtime during testing | Medium | High | Test during stable hours, have backup plan |
| R-002 | Test data not persisting between sessions | High | Medium | Document all test data, recreate as needed |
| R-003 | Browser compatibility issues | Low | Medium | Test on multiple browsers early |
| R-004 | Limited access to logs/backend | High | Low | Focus on UI/functional testing only |
| R-005 | Demo environment limitations | High | Medium | Accept demo limitations, document assumptions |

### 9.2 Assumptions
- Application will remain available throughout testing period
- Demo environment behavior represents intended functionality
- No access to backend/database for verification
- Test data can be created as needed
- No payment processing will be tested (not implemented)

### 9.3 Dependencies
- Stable internet connection
- Application uptime and availability
- Browser compatibility maintained by application
- No major application updates during test execution

---

## 10. Test Metrics & KPIs

### 10.1 Metrics to Track
- **Total Test Cases:** Count of all designed test cases
- **Test Cases Executed:** Number of executed test cases
- **Pass Rate:** (Passed / Executed) × 100
- **Defect Density:** Defects per module
- **Test Coverage:** Features covered / Total features
- **Execution Progress:** Daily execution rate

### 10.2 Success Criteria
- ✅ Pass rate ≥ 95%
- ✅ All critical features tested
- ✅ No critical/high severity bugs open
- ✅ Test coverage ≥ 90% for in-scope features

---

## 11. Communication Plan

### 11.1 Status Reporting
- **Daily:** Informal status via email/chat
- **Weekly:** Formal status report (if applicable)
- **Ad-hoc:** Critical issues reported immediately

### 11.2 Escalation Path
1. **Level 1:** QA Tester (Maciej Miszewski)
2. **Level 2:** QA Lead / Project Manager
3. **Level 3:** Stakeholder / Product Owner

---

## 12. Test Suspension & Resumption Criteria

### 12.1 Suspension Criteria
Testing will be suspended if:
- Application becomes unavailable for >2 hours
- Critical functionality is broken
- Test environment is compromised
- More than 50% of test cases blocked

### 12.2 Resumption Criteria
Testing will resume when:
- Application is restored and stable
- Blocking issues are resolved
- Test environment is validated
- Approval from QA Lead obtained

---

## 13. Defect Management

### 13.1 Defect Lifecycle
1. **New:** Bug discovered and logged
2. **Assigned:** Assigned to developer
3. **In Progress:** Developer working on fix
4. **Fixed:** Developer completed fix
5. **Retest:** QA validates fix
6. **Closed:** Bug verified as fixed
7. **Reopened:** Bug still exists

### 13.2 Severity Definitions
- **Critical:** Application crash, data loss, security issue
- **High:** Major feature broken, no workaround
- **Medium:** Feature issue, workaround available
- **Low:** Minor UI/cosmetic issue

### 13.3 Priority Definitions
- **P1 - Critical:** Fix immediately
- **P2 - High:** Fix in current sprint
- **P3 - Medium:** Fix in next sprint
- **P4 - Low:** Fix when time permits

---

## 14. Approvals

| Role | Name | Signature | Date |
|------|------|-----------|------|
| QA Lead | Maciej Miszewski | ✅ Approved | Jan 15, 2026 |
| Project Manager | [Name] | ✅ Approved | Jan 15, 2026 |
| Stakeholder | [Name] | ✅ Approved | Jan 15, 2026 |

---

## 15. Document History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | Jan 15, 2026 | Maciej Miszewski | Initial test plan created |
| 1.1 | Jan 24, 2026 | Maciej Miszewski | Updated with final test results |

---

## Appendix A: References
- Test Strategy Document
- Test Case Specification
- Demoblaze User Guide (if available)
- Project Requirements Document

## Appendix B: Glossary
- **AUT:** Application Under Test
- **UAT:** User Acceptance Testing
- **SUT:** System Under Test
- **TC:** Test Case
- **TS:** Test Scenario
