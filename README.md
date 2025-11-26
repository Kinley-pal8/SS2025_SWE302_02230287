# SWE302: Software Testing & Quality Assurance

Welcome to the practical repository for **SWE302: Software Testing & Quality Assurance** (SS2025). This repository contains all hands-on practical work for the module, demonstrating real-world implementation of software testing techniques, quality assurance methodologies, and test automation strategies.

**Student:** Kinley Palden  
**Module Code:** SWE302  
**Semester:** Spring/Summer 2025  
**Module Tutor:** Douglas Sim

---

## 📖 Module Overview

### **General Objectives**

This module provides a comprehensive understanding of software testing and quality assurance principles and practices. Students will learn various testing techniques, from unit testing to system testing, and understand how to design tests for different levels of the software development process. The module covers both manual and automated testing approaches, emphasizing the importance of quality throughout the software development lifecycle. Students will gain practical experience in using testing tools, writing test cases, and implementing testing strategies in real-world scenarios.

### **Key Learning Outcomes**

By completion of this module, students will be able to:

1. Explain the fundamental principles of software testing and quality assurance
2. Design and implement effective test cases using specification-based and structural testing techniques
3. Apply property-based testing to uncover edge cases and improve test coverage
4. Utilize test doubles and mocks effectively in unit testing
5. Implement test-driven development (TDD) practices in software development
6. Design software components with testability in mind
7. Develop and execute larger tests, including integration and system tests
8. Evaluate and improve the quality of test code
9. Perform manual exploratory testing to uncover defects not found by automated tests
10. Conduct various types of testing including data, visual, security, performance, and accessibility testing
11. Apply cross-functional requirements testing to ensure overall software quality

---

## 📂 Repository Structure

```
SS2025_SWE302_02230287/
├── README.md                           # This file
├── practicals/                         # All practical sessions
│   ├── practical_1/                    # Testing fundamentals & test design
│   │   └── readme.md
│   ├── practical_2/                    # Unit testing & test doubles
│   │   └── readme.md
│   ├── practical_3/                    # Test-driven development (TDD)
│   │   └── readme.md
│   ├── practical_4/                    # Automated testing tools
│   │   └── readme.md
│   ├── practical_4a/                   # Security testing & vulnerability assessment
│   │   ├── readme.md
│   │   └── zap-baseline-report/
│   ├── practical_4b/                   # Security testing (advanced)
│   │   ├── readme.md
│   │   ├── zap-full-report/
│   │   └── screenshots/
│   ├── practical_5/                    # Integration & system testing
│   │   └── readme.md
│   ├── practical_6/                    # Performance & load testing
│   │   └── readme.md
│   ├── practical_7/                    # Exploratory & manual testing
│   │   └── readme.md
│   ├── practical_8/                    # Test quality & continuous integration
│   │   ├── readme.md
│   │   └── screenshots/
│   └── [Additional materials]
└── [Other course materials]

```

---

## 🎯 Practicals Overview

### **Practical 1: Testing Fundamentals & Test Design**

- **Focus:** Introduction to testing principles and test case design
- **Topics:** Specification-based testing, structural testing, test planning
- **Deliverables:** Well-designed test cases and test plan documentation
- **[View Details](./practicals/practical_1/readme.md)**

### **Practical 2: Unit Testing & Test Doubles**

- **Focus:** Unit testing frameworks and mocking strategies
- **Topics:** JUnit/pytest, test fixtures, mocks, stubs, spies
- **Deliverables:** Comprehensive unit tests with proper test doubles
- **[View Details](./practicals/practical_2/readme.md)**

### **Practical 3: Test-Driven Development (TDD)**

- **Focus:** Red-Green-Refactor cycle and TDD practices
- **Topics:** TDD workflow, design patterns, code quality
- **Deliverables:** Application developed using TDD methodology
- **[View Details](./practicals/practical_3/readme.md)**

### **Practical 4: Automated Testing Tools**

- **Focus:** Test automation frameworks and tools
- **Topics:** Selenium, Cypress, automated UI testing, CI/CD integration
- **Deliverables:** Automated test suite with reporting
- **[View Details](./practicals/practical_4/readme.md)**

### **Practical 4a: Security Testing & Vulnerability Assessment**

- **Focus:** Basic security testing and vulnerability scanning
- **Topics:** OWASP Top 10, security testing methodologies, vulnerability reporting
- **Tools:** OWASP ZAP (baseline scan)
- **Deliverables:** Security test report with findings and recommendations
- **[View Details](./practicals/practical_4a/readme.md)**

### **Practical 4b: Advanced Security Testing**

- **Focus:** Advanced security testing and penetration testing
- **Topics:** Advanced vulnerability assessment, comprehensive security analysis
- **Tools:** OWASP ZAP (full scan), security test reports
- **Deliverables:** Detailed security assessment and remediation plan
- **[View Details](./practicals/practical_4b/readme.md)**

### **Practical 5: Integration & System Testing**

- **Focus:** Testing at integration and system levels
- **Topics:** Integration test strategies, system testing, end-to-end testing
- **Deliverables:** Integration and system test plans with execution results
- **[View Details](./practicals/practical_5/readme.md)**

### **Practical 6: Performance & Load Testing**

- **Focus:** Performance testing and scalability assessment
- **Topics:** Load testing, stress testing, performance metrics, bottleneck identification
- **Deliverables:** Performance test report with analysis and recommendations
- **[View Details](./practicals/practical_6/readme.md)**

### **Practical 7: Exploratory & Manual Testing**

- **Focus:** Exploratory testing and manual QA techniques
- **Topics:** Test charters, bug hunting, user scenarios, edge case discovery
- **Deliverables:** Bug reports and exploratory testing findings
- **[View Details](./practicals/practical7/readme.md)**

### **Practical 8: Test Quality & Continuous Integration**

- **Focus:** Test quality assessment and CI/CD integration
- **Topics:** Test coverage metrics, test code quality, automated test pipelines
- **Deliverables:** CI/CD setup with automated testing and coverage reports
- **[View Details](./practicals/practical_8/readme.md)**

---

## 🛠️ Technology Stack

### **Testing Frameworks & Tools**

| Component               | Technology             | Purpose                 |
| ----------------------- | ---------------------- | ----------------------- |
| **Unit Testing**        | JUnit/pytest/Jasmine   | Unit test execution     |
| **Mocking Framework**   | Mockito/unittest.mock  | Test double creation    |
| **BDD Framework**       | Cucumber/Behave        | Behavior-driven testing |
| **UI Automation**       | Selenium/Cypress       | Web application testing |
| **Security Testing**    | OWASP ZAP              | Vulnerability scanning  |
| **Performance Testing** | JMeter/Locust          | Load and stress testing |
| **CI/CD Platform**      | Jenkins/GitHub Actions | Continuous integration  |
| **Code Coverage**       | JaCoCo/Coverage.py     | Coverage analysis       |
| **Test Reporting**      | Allure/ReportPortal    | Test result reporting   |

### **Development Languages**

- Java, Python, JavaScript (depending on practical requirements)
- Supporting tools and frameworks for each language

---

## ⚙️ Quick Start

### **Prerequisites**

Ensure you have the following installed:

```bash
# Core tools
java -version             # Java 11 or higher
python --version          # Python 3.8 or higher
node --version            # Node.js (for JavaScript practicals)
git --version             # Git for version control
```

### **Clone and Navigate**

```bash
git clone https://github.com/Kinley-pal8/SS2025_SWE302_02230287.git
cd SS2025_SWE302_02230287
```

### **Run a Practical**

```bash
# Navigate to a practical directory
cd practicals/practical_3

# Follow the specific practical README
cat readme.md
```

---

## 📚 Key Concepts Covered

### **Testing Levels**

- Unit Testing
- Integration Testing
- System Testing
- Acceptance Testing
- End-to-End Testing

### **Testing Types**

- Functional Testing
- Non-Functional Testing (Performance, Security, Accessibility)
- Manual Testing
- Automated Testing
- Exploratory Testing

### **Testing Techniques**

- Specification-based (Black-box)
- Structural (White-box)
- Property-based Testing
- Boundary Value Analysis
- Equivalence Partitioning

### **Quality Assurance Practices**

- Test-Driven Development (TDD)
- Behavior-Driven Development (BDD)
- Code Review
- Continuous Integration
- Test Automation Strategies

---

## 🔗 Useful Resources

### **Essential Reading**

- Sommerville, I. (2015). _Software Engineering_. Pearson.
- Srinivasan, R. (2023). _Software Testing: From Fundamentals to Automation_.
- Cohn, M. (2009). _Succeeding with Agile: Software Development using Scrum_. Pearson.

### **Online Documentation**

- [JUnit Documentation](https://junit.org/)
- [Pytest Documentation](https://docs.pytest.org/)
- [Selenium Documentation](https://www.selenium.dev/documentation/)
- [OWASP Testing Guide](https://owasp.org/www-project-web-security-testing-guide/)
- [Apache JMeter](https://jmeter.apache.org/)

### **Tools & Platforms**

- [GitHub](https://github.com/)
- [Stack Overflow](https://stackoverflow.com/)
- [OWASP Foundation](https://owasp.org/)

---

## 📝 Submission Guidelines

### **For Each Practical**

1. **Complete the implementation** as specified in the practical requirements
2. **Document your work** in the practical README with:
   - Brief overview of what was accomplished
   - Screenshots of test execution and results
   - How to run tests and reproduce findings
   - Key learnings and observations
3. **Include evidence** of working tests (screenshots, logs, reports)
4. **Push to GitHub** regularly with meaningful commit messages
5. **Maintain clean code** following best practices for your language

## 🔄 Getting Help

### **During Practicals**

- Review the specific practical's README.md
- Check provided code examples and documentation
- Refer to the module's learning materials on the learning platform

### **Common Issues**

**Test framework not working?**

```bash
# For Python
pip install pytest pytest-mock

# For Java
mvn test

# For JavaScript
npm test
```

**Security tool setup issues?**

```bash
# OWASP ZAP
# Download from https://www.zaproxy.org/
# Follow platform-specific installation guide
```

---

## 📈 Learning Path

```
Practical 1: Testing Fundamentals
    ↓
Practical 2: Unit Testing & Mocks
    ↓
Practical 3: Test-Driven Development
    ↓
Practical 4: Test Automation Tools
    ↓
Practical 4a/4b: Security Testing
    ↓
Practical 5: Integration Testing
    ↓
Practical 6: Performance Testing
    ↓
Practical 7: Exploratory Testing
    ↓
Practical 8: CI/CD & Test Quality
```

Each practical builds upon the concepts from previous ones, creating a comprehensive journey through software testing and quality assurance.

---

## 📂 File Organization Tips

- Keep each practical in its own directory
- Include screenshots in `screenshots/` subdirectories
- Maintain a `readme.md` documenting your implementation
- Use `.gitignore` to exclude build artifacts and dependencies
- Make regular commits with descriptive messages
- Include test reports in the practical folder

---

## 🎓 Acknowledgments

This module is based on industry best practices and current software testing standards. All practicals are designed to provide hands-on experience with real-world testing techniques, tools, and methodologies used in professional software development environments.

---

## 📄 License

This repository and all practical work are part of academic coursework for SWE302.

---
