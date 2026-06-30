# CS 305: Software Security

This repository contains the completion of my security assessments and secure coding practices for **Artemis Financial**, an organization that develops individualized financial plans for customers. 

## Included Artifacts
- `Artemis Financial Vulnerability Assessment Report`
- `Artemis Financial Practices for Secure Software Report`

---

## Project Reflection

**Briefly summarize your client, Artemis Financial, and its software requirements. Who was the client? What issue did the company want you to address?**
Artemis Financial is a consulting company that develops individualized financial plans for customers. Because they handle sensitive financial data, their primary issue was ensuring the security and integrity of their web application. They required a software security overhaul to modernize their operations, specifically requesting the implementation of secure communications (HTTPS/SSL), data integrity verification (checksums), and a comprehensive vulnerability assessment of their software dependencies.

**What did you do well when you found your client's software security vulnerabilities? Why is it important to code securely? What value does software security add to a company's overall well-being?**
I successfully utilized dependency scanning tools to identify critical vulnerabilities within the application's underlying frameworks and libraries. Coding securely is absolutely paramount because it prevents unauthorized access and data breaches, which can devastate an organization. Software security adds immense value to a company's well-being by protecting customer trust, ensuring compliance with data privacy regulations, and avoiding the catastrophic financial and reputational costs associated with cyberattacks.

**Which part of the vulnerability assessment was challenging or helpful to you?**
The most helpful part of the vulnerability assessment was using the OWASP Dependency-Check tool, as it clearly illuminated how outdated external libraries can introduce severe risks into an otherwise secure codebase. The most challenging aspect was determining the correct mitigation strategies for each vulnerability and configuring the secure certificates without breaking the application's core functionality.

**How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?**
I increased layers of security by implementing cryptographic algorithms (SHA-256) to ensure data payload integrity and configuring a self-signed SSL certificate using a keystore to encrypt data in transit via HTTPS. In the future, I would continue to use a combination of Static Application Security Testing (SAST) tools, regular dependency audits (like Maven Dependency-Check), and industry-standard CVE databases to assess vulnerabilities and guide my mitigation strategies.

**How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?**
To ensure functionality, I ran the application locally and verified that the custom checksums were generated accurately and that the web server successfully accepted secure HTTPS requests on the designated port. After refactoring the code to add these security layers, I re-ran the OWASP Dependency-Check against the new build to confirm that no new vulnerable libraries were introduced and that the baseline security posture remained uncompromised.

**What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?**
Integrating the `dependency-check-maven` plugin into the build lifecycle was incredibly valuable and will be a standard practice in my future projects. Additionally, utilizing the Java `keytool` utility for generating SSL keystores and adhering to secure coding guidelines from OWASP are practices that I will carry forward into all future software engineering tasks.

**Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?**
I would gladly show future employers the **Vulnerability Assessment Report** and the refactored **Secure Software** codebase. The report demonstrates my ability to analytically identify, rank, and document security risks, while the code serves as a practical, hands-on example of my ability to implement applied cryptography and secure server configurations to actively mitigate those risks in a Spring Boot application.
