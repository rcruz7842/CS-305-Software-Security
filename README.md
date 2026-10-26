# CS-305 Software Security

This repository contains my work for CS-305 Software Security at Southern New Hampshire University.

## Course Project

### Artemis Financial

For this project, I worked on improving the security of a Java application for Artemis Financial. I reviewed the application for vulnerabilities, added SHA-256 checksum verification, configured HTTPS using a self-signed certificate, and tested the application afterward. I also used OWASP Dependency-Check to identify vulnerabilities in the project's dependencies.

[Practices for Secure Software Report](Artemis%20Financial/Artemis%20Financial%20Practices%20for%20Secure%20Software%20Report.docx)

### Technologies and Concepts
- Java
- Spring Boot
- SHA-256
- HTTPS and SSL/TLS certificates
- Java Keytool
- OWASP Dependency-Check
- Secure coding and vulnerability testing

## Portfolio Reflection

### Identifying Security Vulnerabilities
I did well with finding areas of the application that needed better security and figuring out what could be done to improve them. I added things like SHA-256 checksum verification and HTTPS, and then tested the application afterward to make sure everything was still working correctly. Adding security during the coding process instead of waiting until after makes it easier to catch vulnerabilities before they become bigger problems. Coding securely is important since any vulnerabilities can put sensitive information at risk. For a company like Artemis Financial, having secure software protects their clients' information as well as prevents security problems that could affect the company itself.

### Working with OWASP Dependency-Check
The OWASP Dependency-Check was one of the more challenging, yet helpful parts of the vulnerability assessment. Seeing a large number of vulnerabilities in the dependencies at first was a little overwhelming, but it helped me understand how vulnerabilities can come from third-party dependencies and not just the code. It showed me *why* checking dependencies is an important part of keeping an application secure.

### Adding Layers of Security
I added more layers of security throughout the application instead of relying solely on one security method. I used SHA-256 to verify that data wasn't changed and configured HTTPS to protect the connection between the browser and server. I created a certificate and keystore for the HTTPS connection and used the OWASP Dependency-Check to check for vulnerabilities in the dependencies. In the future, I would start by looking at where the vulnerabilities are coming from first and then how they could affect the application before deciding on the best way to fix it.

### Testing After Refactoring
After refactoring the code, I didn't want to assume that everything was secure just because the changes worked. I tested the SHA-256 checksum to make sure it was generating correctly and opened the /hash page through HTTPS to verify the secure connection was still working. I also manually reviewed the code for any errors and ran the OWASP Dependency-Check again to see if the changes introduced any new vulnerabilities. Testing everything again helped confirm that the application still worked correctly after the security changes were made.

### Tools and Resources
Working with the OWASP Dependency-Check was helpful since I could see vulnerabilities that I wouldn't have found just by going through the code myself. I also got more practice with Java Keytool when creating the certificate and learned how Java's security libraries could be used for things like SHA-256. These are tools I can see myself using again, especially when I need to check the security of an application instead of only focusing on whether the code works.

### Applying What I Learned
This project would be a good example to show future employers because it includes the actual security changes I made to the application and how I tested them afterward. It shows my work with HTTPS, certificates, SHA-256, and finding vulnerabilities with the OWASP Dependency-Check. It also shows that I can work through security problems, make the changes that are needed, and test everything afterward to make sure it still works.
