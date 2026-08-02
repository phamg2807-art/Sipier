# Security Policy

## Sipier Automation Suite

Security is important to the Sipier project.

Sipier is currently in **Beta testing** and is actively being developed. We take security reports seriously and appreciate the efforts of security researchers, developers, and users who help identify potential vulnerabilities.

This document explains how to report security vulnerabilities and what information should be included in a security report.

---

# Supported Versions

Sipier is currently under active development.

Security fixes are generally prioritized for:

| Version                | Supported   |
| ---------------------- | ----------- |
| Latest Beta Release    | Yes         |
| Previous Beta Releases | Limited     |
| Development Builds     | Best Effort |
| Unmaintained Releases  | No          |

Because Sipier is still in Beta, the supported version policy may change as the project matures.

Users are strongly encouraged to use the latest official release when possible.

---

# Reporting a Security Vulnerability

If you discover a potential security vulnerability in Sipier, please report it responsibly.

**Do not immediately publish the vulnerability publicly.**

Publicly disclosing an unpatched vulnerability may put other users at unnecessary risk.

Instead, please contact the Sipier development team through the security reporting mechanism provided by the official GitHub repository.

If GitHub Security Advisories are enabled for the repository, please use the **Private Vulnerability Reporting** feature.

If private reporting is not available, contact the project maintainers through the official contact method listed in the repository.

---

# What Should Be Reported?

Please report security issues that could affect the confidentiality, integrity, or availability of users, their data, or their systems.

Examples may include:

* Unauthorized access to user data.
* Unexpected collection of sensitive information.
* Credential exposure.
* Password or token leakage.
* Arbitrary code execution.
* Privilege escalation.
* Unsafe file handling.
* Malicious file loading.
* Unexpected network communication.
* Remote code execution.
* Insecure update mechanisms.
* Authentication or authorization vulnerabilities.
* Sensitive information disclosure.
* Vulnerabilities in application components.
* Vulnerabilities introduced by Sipier's own code.

If you are unsure whether an issue qualifies as a security vulnerability, please report it anyway.

We would rather investigate a potentially valid report than have a legitimate security issue go unnoticed.

---

# What Does Not Usually Qualify as a Security Vulnerability?

The following issues are generally not considered security vulnerabilities by themselves:

* Normal application bugs.
* UI issues.
* Visual glitches.
* Performance problems.
* Feature requests.
* Incorrect macro behavior.
* General crashes without security impact.
* Windows SmartScreen warnings caused by an unsigned application.
* Unknown publisher warnings.
* Antivirus false positives without evidence of malicious behavior.

These issues should generally be reported through regular GitHub Issues.

However, if you believe an issue has a genuine security impact, please explain why in your report.

---

# Windows Defender and Antivirus Reports

Sipier is automation software and may interact with mouse, keyboard, window, and system functionality.

Security software may occasionally identify legitimate automation behavior as suspicious.

If you believe Sipier has been incorrectly detected as malware, please report the detection.

Include:

* Sipier version.
* Windows version.
* Exact antivirus product.
* Exact detection name.
* File name.
* File hash, if available.
* Where the file was downloaded from.
* Relevant screenshots.

Do not simply disable security software and assume the detection is incorrect.

The development team will investigate the report and determine whether it appears to be a false positive or a legitimate security concern.

For more information about Windows security warnings, see:

`APPSAFETY.md`

---

# Security Report Contents

A useful security report should contain as much technical information as possible.

Please include:

### 1. Vulnerability Description

Explain what the vulnerability is.

### 2. Affected Version

Specify which version or versions are affected.

### 3. Steps to Reproduce

Provide clear steps that allow the development team to reproduce the issue.

### 4. Expected Behavior

Explain what you expected the application to do.

### 5. Actual Behavior

Explain what the application actually did.

### 6. Security Impact

Explain what an attacker could potentially accomplish.

### 7. Proof of Concept

If available, provide a minimal proof of concept.

Only provide proof-of-concept code that is necessary to demonstrate the vulnerability.

### 8. Additional Information

Include any relevant:

* Logs.
* Screenshots.
* Error messages.
* Stack traces.
* File hashes.
* System information.

Please remove passwords, API keys, tokens, and other sensitive information before submitting your report.

---

# Example Security Report

A useful report might look like:

```text
Title:
Potential arbitrary file execution through macro import

Affected Version:
Sipier Beta 0.1.0

Description:
A specially crafted macro file may cause Sipier to execute an unexpected
local file when imported.

Steps to Reproduce:
1. Launch Sipier.
2. Open the macro import feature.
3. Import the attached test file.
4. Observe the unexpected behavior.

Expected Behavior:
Sipier should only import valid macro data.

Actual Behavior:
The application attempts to process an unexpected file path.

Security Impact:
An attacker who can convince a user to import a maliciously crafted
macro file may potentially cause unintended local actions.

Environment:
Windows 11
Sipier Beta 0.1.0

Additional Information:
Attached logs and screenshots.
```

---

# Responsible Disclosure

We encourage responsible disclosure.

If you discover a vulnerability:

1. Report it privately.
2. Allow the development team reasonable time to investigate.
3. Allow the issue to be fixed where possible.
4. Coordinate public disclosure with the development team.

Please avoid:

* Publicly posting exploit instructions before a fix is available.
* Using the vulnerability against other users.
* Accessing data that does not belong to you.
* Destroying or modifying user data.
* Performing unnecessary denial-of-service testing.
* Social engineering project contributors.
* Attempting to gain unauthorized access to project infrastructure.

Security research should be performed responsibly and ethically.

---

# Security Research Guidelines

Security researchers are encouraged to minimize the potential impact of their testing.

When investigating Sipier:

* Test only systems you own or have permission to test.
* Use isolated test environments when possible.
* Avoid accessing personal data.
* Avoid collecting credentials.
* Avoid persistent modifications.
* Avoid destructive testing.
* Avoid disrupting services.
* Stop testing if you discover evidence of active exploitation.

The goal of security research is to improve security, not to cause harm.

---

# Third-Party Dependencies

Sipier uses third-party software and libraries.

Security vulnerabilities may exist in dependencies independently of Sipier's own source code.

If you discover a vulnerability in a third-party dependency used by Sipier, please:

1. Determine whether the vulnerability affects Sipier.
2. Check whether an updated version of the dependency is available.
3. Report the issue to the relevant third-party project when appropriate.
4. Inform the Sipier development team if the vulnerability affects Sipier users.

Please do not assume that every third-party vulnerability automatically affects Sipier.

---

# Supply Chain Security

The Sipier project recognizes the importance of software supply-chain security.

Potential risks include:

* Compromised dependencies.
* Malicious packages.
* Compromised developer accounts.
* Modified release artifacts.
* Compromised build systems.
* Unauthorized repository changes.

The project may introduce additional security controls as development progresses.

Potential future measures include:

* Dependency vulnerability scanning.
* Automated security checks.
* Signed commits.
* Protected branches.
* Release checksums.
* Code signing.
* Reproducible builds.
* Automated build pipelines.
* GitHub security features.

---

# Release Security

Users should download Sipier only from official release channels.

Official releases should be distributed through the project's GitHub repository.

Users should be cautious of unofficial copies distributed through:

* Unknown websites.
* Unofficial file hosts.
* Modified builds.
* Pirated software websites.
* Unknown Discord servers.
* Unverified social media accounts.
* Third-party download sites.

If you discover an unofficial version claiming to be Sipier, please report it to the project maintainers.

---

# Code Signing

Sipier is currently in Beta and may not have a trusted commercial code-signing certificate.

As a result, Windows may display publisher verification warnings.

Code signing may be introduced for future stable releases.

Code signing helps verify:

* The identity of the publisher.
* The integrity of the signed executable.

However, a valid code signature does not guarantee that software is completely secure.

Security remains a continuous process.

---

# Security Updates

When a security vulnerability is confirmed, the development team will evaluate its severity and determine an appropriate response.

Depending on the issue, the response may include:

* A code fix.
* A dependency update.
* A configuration change.
* A new release.
* A security advisory.
* Documentation updates.

Users may be encouraged to update to the latest version when a security fix becomes available.

---

# Security Advisory Process

For significant vulnerabilities, the project may publish a security advisory containing:

* Affected versions.
* Fixed versions.
* Vulnerability description.
* Severity information.
* Mitigation instructions.
* Upgrade recommendations.

Sensitive exploit details may be withheld until users have had a reasonable opportunity to update.

---

# Severity

Security issues may be evaluated based on factors such as:

* Potential impact.
* Exploitability.
* Required user interaction.
* Required privileges.
* Attack complexity.
* Number of affected users.

Severity classifications may include:

* Critical
* High
* Medium
* Low
* Informational

The final severity assessment is determined by the project maintainers.

---

# Response Process

When a valid security report is received, the development team will attempt to:

1. Acknowledge receipt of the report.
2. Review the reported behavior.
3. Reproduce the issue.
4. Determine whether it is a vulnerability.
5. Evaluate the potential impact.
6. Identify affected versions.
7. Develop a fix where possible.
8. Test the fix.
9. Release the fix.
10. Communicate relevant information to users.

Response times may vary depending on:

* Vulnerability complexity.
* Available development resources.
* Required investigation.
* Severity of the issue.

Sipier is an independent Beta project, so response times cannot always be guaranteed.

---

# Security Researcher Recognition

With permission, security researchers who responsibly report valid vulnerabilities may be recognized in project release notes or security acknowledgements.

Researchers who do not wish to be publicly recognized may request anonymity.

No personal information will be publicly disclosed without permission.

---

# Safe Harbor

Security researchers acting in good faith and following this policy should not be subject to legal action by the Sipier project for security research conducted within the scope of this policy.

This safe harbor applies only to activities that:

* Follow applicable laws.
* Are conducted in good faith.
* Avoid unnecessary harm.
* Avoid accessing data that does not belong to the researcher.
* Avoid disrupting other users.
* Follow responsible disclosure practices.

This policy does not authorize testing against systems or infrastructure that you do not own or have permission to test.

---

# Scope

This security policy applies primarily to:

* Sipier source code.
* Official Sipier releases.
* Official Sipier installers.
* Official Sipier distribution mechanisms.
* Security-related project infrastructure where applicable.

Third-party services and dependencies may have their own security policies.

---

# Privacy

When submitting a security report, please avoid including unnecessary personal information.

Do not include:

* Passwords.
* API keys.
* Authentication tokens.
* Private documents.
* Personal identification information.
* Unrelated sensitive data.

If sensitive information is accidentally included in a report, notify the project maintainers as soon as possible.

---

# Disclaimer

Sipier is currently Beta software.

The project does not guarantee that the application is completely free from security vulnerabilities.

No software can guarantee absolute security.

This policy exists to provide a responsible process for identifying and addressing security issues.

We encourage users and researchers to report suspicious behavior and potential vulnerabilities so that Sipier can become safer over time.

---

# Contact

For security-related issues, please use the private security reporting mechanism provided by the official Sipier GitHub repository whenever possible.

For general bugs and feature requests, please use GitHub Issues instead.

For security issues, **do not publicly disclose sensitive vulnerability details in a normal GitHub Issue**.

---

# Thank You

Security is a shared responsibility.

We appreciate everyone who takes the time to responsibly report vulnerabilities, investigate suspicious behavior, test new releases, and help improve the security of Sipier.

Your contributions help protect the Sipier community and make the project stronger.

**Thank you for helping make Sipier safer.**
