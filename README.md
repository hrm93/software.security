# software.security
for CS-305

# Briefly summarize your client, Artemis Financial, and its software requirements. Who was the client? What issue did the company want you to address?
**Client**: Artemis Financial

**Business**: Artemis Financial is a consulting company specializing in developing individualized financial plans for its clients. 
These plans encompass savings, retirement, investments, and insurance, aiming to provide tailored financial advice and strategies to meet the unique needs of each client.

**Issue**: Artemis Financial sought to modernize its operations by upgrading its existing software systems. They required a comprehensive security overhaul to protect sensitive financial data from external threats. 
This included ensuring secure communications, safeguarding international transactions, complying with governmental regulations, and mitigating various security vulnerabilities.

**Software Requirements**

-Secure Communications: Implement robust encryption standards like TLS 1.3 to protect data in transit.

-International Transaction Security: Ensure data protection and compliance with international data protection regulations for cross-border transactions.

-Compliance with Governmental Restrictions: Adhere to data protection laws such as GDPR, CCPA, and SOX.

-Protection Against External Threats: Guard against phishing, SQL injection, XSS, MITM attacks, APTs, and zero-day vulnerabilities.

-Modernization: Incorporate the use of open-source libraries, secure coding practices for evolving web technologies, and automated security testing.

# What did you do well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall well-being?
**Success in Finding Vulnerabilities:**

**Approach**: Conducted a thorough vulnerability assessment that included both manual code reviews and static analysis.
Identified various security weaknesses such as potential SQL injection points, insecure database connection handling, insufficient input validation, hardcoded strings, and outdated dependencies with known vulnerabilities.

**Outcome**: Documented the findings in a detailed vulnerability assessment report and provided actionable recommendations for mitigation.

**Importance of Secure Coding**

-Data Integrity: Secure coding practices ensure that data remains accurate and unaltered during processing and storage.

-Confidentiality: Protecting sensitive information from unauthorized access prevents data breaches.

-Compliance: Ensuring the software adheres to regulatory standards (e.g., GDPR, CCPA) helps avoid legal repercussions and fines.

**Value of Software Security**

-Protection: Safeguards sensitive financial data from breaches, cyber-attacks, and other security incidents.

-Trust: Builds and maintains client trust by ensuring their information is secure, which is critical for client retention and business reputation.

-Compliance: Helps meet regulatory requirements, ensuring the company operates within the law and avoids penalties.

# Which part of the vulnerability assessment was challenging or helpful to you?
**Challenges:**

-Dependency Vulnerabilities: Updating multiple third-party libraries without breaking existing functionality required careful planning and testing. Ensuring compatibility with the rest of the codebase while patching vulnerabilities was particularly challenging.

-Input Validation: Comprehensive input validation to cover all potential injection points and edge cases required thorough analysis and testing.

**Helpful Aspects:**

-Automated Tools: Using tools like static analysis and dependency checkers provided a clear and systematic identification of vulnerabilities. These tools offered valuable insights and recommendations that facilitated the mitigation process.

# How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?
**Actions Taken:**

-Architecture Review: Conducted an in-depth review of the application’s architecture to identify and rectify structural weaknesses.

-Input Validation: Implemented strict validation and sanitization for all user inputs to prevent injection attacks.

-API Security: Secured APIs with OAuth for authentication and rate limiting to prevent abuse.

-Cryptography: Used strong encryption methods (AES-256 for data at rest and TLS 1.3 for data in transit) to protect sensitive information.

-Concurrency Handling: Ensured thread safety in concurrent operations using appropriate synchronization mechanisms.

-Error Handling: Implemented proper error handling to prevent information leakage through error messages.

-Logging: Added logging to record significant events, errors, and security incidents using a secure logging framework.

**Future Assessments:**

-Continuous Integration/Continuous Deployment (CI/CD): Implement automated security testing within CI/CD pipelines to detect vulnerabilities early.

-Security Tools: Continue using static analysis tools, dependency checkers, and manual code reviews.

-Threat Modeling: Use threat modeling techniques to anticipate potential attack vectors and design defenses accordingly.

# How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?
**Methods:**

-Refactoring: Refactored the code to remove identified vulnerabilities, ensuring adherence to secure coding practices.

-Testing: Conducted rigorous testing including unit tests, integration tests, and security tests to verify both functionality and security.

-Automated Tools: Re-scanned the codebase with automated tools after refactoring to detect any new vulnerabilities introduced during the changes.

**Validation:**

-Post-Refactoring: Ensured that the application remained functional and secure after changes by running comprehensive test suites and verifying that no new vulnerabilities were present.

# What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?
**Resources and Tools:**

-Static Analysis Tools: Utilized for identifying vulnerabilities in the codebase.

-Dependency Checkers: Tools like Dependabot and Snyk to monitor and manage third-party library vulnerabilities.

-Secure Coding Guidelines: Followed industry best practices for secure coding, including input validation, encryption, and error handling.

**Helpful Practices:**

-Code Reviews: Regular code reviews and pair programming sessions to catch potential security issues early.

-Continuous Learning: Staying updated with the latest security trends, best practices, and emerging threats.

# Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?
**Portfolio Elements:**

-Vulnerability Assessment Report: Detailed documentation of identified vulnerabilities, their impacts, and mitigation strategies.

-Refactored Code Samples: Demonstrated improvements and secure coding practices applied to the original code.

-Dependency Management: Example of using automated tools to manage and update dependencies.

-Security Testing Evidence: Documentation of rigorous testing and validation processes to ensure both functionality and security of the application.

These elements showcase your capability in conducting thorough security assessments, implementing effective mitigation strategies, and maintaining secure and functional software.
