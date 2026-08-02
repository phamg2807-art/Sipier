## Windows Defender / SmartScreen Warning

<img width="504" height="295" alt="image" src="https://github.com/user-attachments/assets/314550d5-f16f-446d-9d19-7991b6d8716b" />



# Sipier Security, Privacy, Safety and Trust Statement

**Last Updated:** August 3 2026

Sipier Automation Suite is a Windows desktop automation application currently in **Beta Testing**.

This document exists to provide users, developers, security researchers, and the wider community with as much transparency as possible about how Sipier works, how it is distributed, what risks may exist, why Windows may display security warnings, what Sipier can and cannot access, and how users can verify that they are using an authentic release.

Our goal is to build trust through transparency rather than simply asking users to trust an unknown executable.

---

# 1. Introduction

Sipier is a desktop automation and macro application designed to automate repetitive mouse and keyboard workflows.

The application is intended to provide users with tools for creating, recording, managing, and executing automation sequences through a graphical desktop interface.

Sipier is currently in active development.

Because this is a Beta release, the software may contain:

* Bugs
* Unexpected behavior
* Incomplete features
* Performance issues
* Stability problems
* Compatibility problems
* False-positive antivirus detections
* Unintended application behavior

For this reason, Sipier should be treated as **Beta software**.

We do not recommend using Beta software in situations where an unexpected automation action could cause significant damage, data loss, financial loss, or other serious consequences.

---

# 2. Our Security Philosophy

Sipier follows a simple principle:

> **Users should be able to understand what software is doing on their computer.**

We do not expect users to blindly trust an executable simply because it is called Sipier.

Users should have the ability to:

* Review the source code.
* Inspect the project structure.
* Review changes to the project.
* Report security issues.
* Examine release information.
* Verify that they downloaded the application from the official source.
* Understand why Windows may display a warning.
* Decide whether they are comfortable running the application.

The goal of this document is to make that process as transparent as possible.

---

# 3. Is Sipier Malware?

Sipier is developed as a legitimate desktop automation application.

The intended purpose of Sipier is to automate user-defined mouse and keyboard actions.

Sipier is not designed to function as:

* A virus
* A worm
* A ransomware application
* A credential stealer
* A password stealer
* A spyware application
* A remote access trojan
* A cryptocurrency miner
* A botnet client
* A browser hijacker
* A persistence mechanism
* A data exfiltration tool

However, it is important to understand the distinction between **intent** and **verification**.

Sipier is currently a Beta project and has not undergone a formal independent security audit.

Therefore, we do not claim that any software is "100% guaranteed safe" under every possible circumstance.

Instead, we encourage users to review the source code, download releases only from official sources, and report anything suspicious.

---

# 4. Why Does Windows Security Warn About Sipier?

Some users may see a Windows Security message similar to:

> **Part of this app has been blocked**

> Some features of Sipier Automation Suite may not work because we can't confirm who published Sipier.exe that the app tried to load.

Users may also encounter warnings related to:

* Unknown publisher
* Unrecognized application
* Unverified publisher
* Microsoft Defender SmartScreen
* Windows reputation protection

These warnings can be alarming.

It is important to understand that **publisher verification and malware detection are not the same thing**.

Windows may warn users because it cannot establish a trusted identity for the publisher of an executable.

This can happen when an application:

* Is newly released.
* Has a low download count.
* Has not established a reputation with Microsoft's security systems.
* Is not digitally code-signed.
* Uses a self-built executable.
* Is distributed outside the Microsoft Store.
* Is packaged using tools such as PyInstaller.
* Has a publisher identity that Windows cannot verify.

Sipier is currently a new Beta application and may not have an established publisher reputation.

The current release may also not have a trusted commercial code-signing certificate.

As a result, Windows may be unable to verify the identity of the publisher.

This does **not automatically mean that Sipier contains malware**.

However, users should still take security warnings seriously.

---

# 5. Publisher Verification vs. Malware Detection

These are two different situations.

## Publisher Verification Warning

A publisher warning generally means:

> "Windows cannot verify who published this application."

This is related to application identity and digital signatures.

It does not necessarily mean:

> "Windows has detected malware."

## Malware Detection

A malware detection means that Windows Defender or another security product has identified behavior or code that matches a known or suspected threat.

Examples may include:

* Trojan
* Virus
* Spyware
* Ransomware
* Credential theft
* Suspicious behavior

These warnings should be treated much more seriously.

If Windows Defender specifically identifies Sipier as malware, users should **not simply disable Windows Defender and continue**.

Instead, users should report the detection to the Sipier development team so that the issue can be investigated.

---

# 6. Why Automation Software Can Trigger Security Warnings

Automation software sometimes interacts with the operating system in ways that security software considers unusual.

Depending on the features implemented, automation software may interact with:

* Mouse input
* Keyboard input
* Window focus
* Screen coordinates
* Application windows
* Global input events
* System-level input APIs

These capabilities are legitimate for automation software.

However, similar capabilities can also be abused by malicious software.

For example, malware may attempt to:

* Simulate user input.
* Control applications.
* Capture keyboard input.
* Interact with windows.
* Automate malicious actions.

Security software therefore may apply additional scrutiny to applications that perform automation-related behavior.

The fact that Sipier performs automation does not inherently make it malicious.

At the same time, we understand why security software may treat such applications cautiously.

---

# 7. What Sipier Is Intended to Access

Sipier's intended functionality may require access to certain system capabilities necessary for automation.

Depending on the features enabled, Sipier may interact with:

* Mouse input
* Keyboard input
* Screen coordinates
* Window positions
* Application focus
* Local macro configuration
* Local application files

These capabilities exist to provide the core functionality of the application.

Sipier should not require access to unrelated personal information to perform basic macro automation.

---

# 8. What Sipier Is Not Intended to Collect

Sipier is not designed to intentionally collect or steal:

* Passwords
* Authentication tokens
* Browser cookies
* Credit card information
* Banking information
* Private messages
* Personal documents
* Personal photographs
* Webcam recordings
* Microphone recordings
* Browser history
* Private account credentials

Sipier's purpose is automation, not surveillance.

If future functionality requires additional data collection, that functionality should be clearly documented.

---

# 9. Network Activity

Users should be aware of what network functionality is included in the specific Sipier version they install.

If a version of Sipier does not require online services for its functionality, users should not assume that network access is necessary.

If future versions introduce:

* Automatic updates
* Online synchronization
* Cloud storage
* Analytics
* Crash reporting
* Account systems
* Online services

those capabilities should be clearly documented.

Users should always be able to understand why an application communicates with external servers.

---

# 10. Privacy

Sipier is intended to respect user privacy.

The application should not intentionally collect personal information unrelated to its core functionality.

Users should not be required to provide sensitive personal information simply to use basic local automation functionality.

If future versions introduce analytics or telemetry, the collection and purpose of that data should be clearly disclosed.

---

# 11. Local Data

Sipier may store application data locally depending on the features enabled.

This may include:

* Macro configurations
* Automation settings
* Application preferences
* Theme preferences
* User-defined workflows

Users should treat saved macro files as potentially sensitive if they contain information about private workflows.

For example, a macro may contain:

* Application names
* Window positions
* Mouse coordinates
* Keyboard actions
* User-defined text

Users should avoid storing sensitive credentials or passwords inside macros.

---

# 12. Passwords and Sensitive Information

Sipier should never be used as a password storage system.

Users should not create macros containing:

* Passwords
* API keys
* Authentication tokens
* Private keys
* Recovery codes
* Banking information

Automation systems can replay recorded actions.

If sensitive information is embedded into a macro, anyone who gains access to that macro may potentially inspect the stored information.

Users are responsible for protecting their macro files.

---

# 13. Source Code Transparency

Sipier's source code is available through the project's GitHub repository.

Users and developers can inspect the source code to better understand how the application operates.

This allows the community to:

* Review implementation details.
* Identify suspicious behavior.
* Report vulnerabilities.
* Suggest security improvements.
* Verify application functionality.
* Contribute improvements.

We encourage technically experienced users to inspect the source code if they have concerns about the application.

Open source does not automatically guarantee that software is secure.

However, transparency allows independent review and makes it easier for the community to identify potential problems.

---

# 14. Official Releases

Users should download Sipier only from official release channels.

The safest source is the official Sipier GitHub repository and its official Releases section.

Users should avoid downloading Sipier from:

* Unknown websites
* Random file-hosting websites
* Unverified mirrors
* Pirated software websites
* Untrusted Discord links
* Unknown social media attachments
* Unverified third-party repositories

A malicious third party could potentially modify a legitimate application and redistribute it under the same name.

Always verify the source before running an executable.

---

# 15. How to Verify Your Download

Before installing Sipier:

1. Download the application from the official GitHub Release.
2. Check the release version.
3. Compare the filename with the official release information.
4. Make sure the download came directly from the official repository.
5. Scan the downloaded file with your security software.
6. If available, verify the published SHA-256 checksum.
7. Do not use modified or repackaged versions.

Users should never assume that every file named "Sipier.exe" is an official Sipier release.

---

# 16. File Integrity

For future releases, Sipier may provide cryptographic hashes such as SHA-256.

A cryptographic hash allows users to verify that a downloaded file matches the original file published by the development team.

For example:

```text
SHA-256
xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```

If the calculated hash of the downloaded file matches the official published hash, the file contents are identical to the published file.

If the hash does not match, users should not run the file until the discrepancy is investigated.

---

# 17. Code Signing

Sipier is currently a Beta application and may not have a trusted commercial code-signing certificate.

This is one reason Windows may display publisher verification warnings.

A future production release may use code signing to provide:

* Publisher identity verification
* File integrity verification
* Improved Windows trust
* Reduced SmartScreen warnings
* Better protection against modified executables

Code signing is an important part of professional Windows software distribution.

We consider it an important improvement for future stable releases.

---

# 18. What Code Signing Does

Code signing allows a developer or organization to digitally sign an application.

The signature helps Windows verify:

* Who signed the application.
* Whether the application has been modified since signing.

This is different from a security audit.

A valid digital signature does not automatically prove that software is harmless.

It primarily provides publisher identity and integrity verification.

Users should still evaluate software responsibly.

---

# 19. What Sipier Cannot Guarantee

Sipier cannot guarantee:

* That Windows will never display a security warning.
* That every antivirus product will always classify it correctly.
* That Beta software will never contain bugs.
* That every future version will behave identically.
* That third-party repackaged versions are safe.
* That a compromised development environment is impossible.
* That every user's system configuration will be compatible.

No software project can honestly guarantee absolute security.

Our goal is to reduce risk through transparency, secure development practices, careful distribution, and community review.

---

# 20. Beta Software Risks

Sipier is currently Beta software.

Beta software may contain defects that have not yet been discovered.

Possible risks include:

* Application crashes
* Unexpected automation
* Incorrect mouse coordinates
* Incorrect keyboard actions
* Macro loops
* Performance issues
* UI bugs
* Data corruption
* Compatibility problems
* Unexpected behavior

Users should test new macros carefully before using them in important environments.

---

# 21. Automation Safety

Automation can perform actions very quickly and repeatedly.

A poorly configured macro could:

* Click the wrong location.
* Enter incorrect text.
* Repeat an action indefinitely.
* Interact with the wrong application.
* Modify unintended data.

Users should always test automation carefully.

We strongly recommend:

* Testing new macros manually.
* Starting with short execution periods.
* Using reasonable delays.
* Avoiding unattended automation until properly tested.
* Keeping emergency stop functionality accessible.

---

# 22. Emergency Stop

Users should always know how to immediately stop an active automation sequence.

If Sipier provides an emergency stop mechanism, users should familiarize themselves with it before running automation.

If a macro behaves unexpectedly:

1. Stop the automation immediately.
2. Close the target application if necessary.
3. Review the macro configuration.
4. Identify the cause.
5. Correct the macro before running it again.

---

# 23. Antivirus False Positives

Security software occasionally produces false positives.

A false positive occurs when legitimate software is incorrectly identified as suspicious.

This can happen because of:

* New software
* Low reputation
* Unsigned executables
* Application packaging methods
* Automation behavior
* Unusual executable structures

However, not every detection is a false positive.

Therefore, we do not recommend blindly excluding Sipier from antivirus protection.

Instead, users should report the exact detection to the development team.

---

# 24. If Windows Defender Detects Sipier

If Microsoft Defender reports a specific malware detection:

**Do not immediately disable Defender.**

Instead:

1. Record the exact detection name.
2. Note the Sipier version.
3. Confirm where the file was downloaded from.
4. Check whether the file is an official release.
5. Report the detection to the development team.
6. Provide the relevant information so the issue can be investigated.

If the detection is confirmed to be a false positive, the development team can investigate potential causes and work toward resolving the issue.

---

# 25. If Windows Only Says "Unknown Publisher"

An unknown publisher warning is different from a malware detection.

It generally indicates that Windows cannot verify the publisher's identity.

If you downloaded Sipier from the official release page and have independently verified the file's authenticity, you may choose whether to proceed.

However, users should never bypass security warnings for files obtained from unknown sources.

---

# 26. Do Not Disable Windows Security Globally

We strongly discourage users from:

* Permanently disabling Windows Defender.
* Disabling real-time protection.
* Disabling SmartScreen system-wide.
* Adding unknown files to antivirus exclusions.
* Turning off firewall protection.

These actions can expose the entire computer to unnecessary risk.

If you believe Sipier has been incorrectly blocked, investigate the specific warning instead of disabling all security protections.

---

# 27. Responsible Disclosure

If you discover a potential security vulnerability in Sipier, please report it responsibly.

Do not publicly publish exploit details before the issue has been investigated.

Security reports should include:

* A clear description of the vulnerability.
* Steps to reproduce the issue.
* Affected version.
* Expected behavior.
* Actual behavior.
* Potential impact.
* Screenshots or logs when appropriate.
* Proof of concept when safe and necessary.

Do not include private personal information in security reports.

---

# 28. Security Vulnerability Examples

Potential security issues may include:

* Unauthorized data access.
* Unexpected network communication.
* Credential exposure.
* Privilege escalation.
* Arbitrary code execution.
* Unsafe update mechanisms.
* Malicious file loading.
* Unauthorized persistence.
* Data leakage.

If you discover behavior that appears inconsistent with Sipier's intended functionality, report it.

---

# 29. Community Security Review

We welcome responsible security review from developers and security researchers.

The community can help improve Sipier by identifying:

* Security weaknesses.
* Privacy concerns.
* Unsafe dependencies.
* Packaging issues.
* Suspicious behavior.
* Unexpected network activity.
* Vulnerable third-party libraries.

Responsible feedback is encouraged.

---

# 30. Third-Party Dependencies

Sipier may rely on third-party libraries and frameworks.

These dependencies may include libraries used for:

* Graphical interfaces.
* Automation.
* Packaging.
* System interaction.

Third-party dependencies can introduce vulnerabilities independently of Sipier's own code.

Developers should keep dependencies updated where practical and review security advisories affecting the project's dependencies.

---

# 31. Supply Chain Security

Software supply-chain security is an important consideration.

Potential risks can occur through:

* Compromised dependencies.
* Malicious packages.
* Compromised build environments.
* Modified release files.
* Compromised developer accounts.

We recognize that securing the entire software supply chain is an ongoing process.

Future improvements may include:

* Dependency auditing.
* Reproducible builds.
* Automated security scanning.
* Release checksums.
* Signed commits.
* Signed releases.
* Code signing.
* Automated build pipelines.

---

# 32. Release Integrity

Official releases should be distributed through controlled release channels.

The development team should maintain clear version numbers and release notes.

Users should avoid unofficial builds unless they fully trust the person providing them.

If a third party claims to provide an "updated" or "modified" version of Sipier, users should treat it as unofficial.

---

# 33. Privacy and Telemetry Transparency

If Sipier introduces telemetry, analytics, or crash reporting in the future, the project should clearly document:

* What data is collected.
* Why it is collected.
* Where it is stored.
* How long it is retained.
* Whether it can be disabled.
* Whether personal information is collected.

Users deserve to know what information leaves their computer.

---

# 34. No Hidden Behavior Policy

Sipier should not intentionally contain hidden functionality unrelated to its stated purpose.

The project should not intentionally include:

* Hidden malware.
* Credential theft.
* Unauthorized surveillance.
* Secret persistence.
* Undisclosed remote access.
* Undisclosed data collection.

If a security researcher discovers behavior that appears inconsistent with this policy, we encourage them to report it immediately.

---

# 35. User Responsibility

Users are responsible for downloading software from trustworthy sources and using the application responsibly.

Users should:

* Download official releases.
* Keep Windows updated.
* Keep antivirus protection enabled.
* Avoid unofficial modified builds.
* Keep backups of important data.
* Test automation carefully.
* Report suspicious behavior.

Sipier is a tool.

The user is responsible for determining whether and where the tool should be used.

---

# 36. Developer Responsibility

The Sipier development team is responsible for making reasonable efforts to:

* Maintain the project's source code.
* Investigate reported security issues.
* Address confirmed vulnerabilities.
* Avoid unnecessary data collection.
* Communicate important security issues.
* Improve release integrity.
* Improve Windows compatibility.
* Improve application trust and verification.

Security is an ongoing process rather than a one-time feature.

---

# 37. Our Commitment

We understand that running an unknown executable on a personal computer requires trust.

We do not expect users to trust Sipier blindly.

Instead, we encourage users to:

* Inspect the source code.
* Review release history.
* Verify downloads.
* Check security warnings.
* Report suspicious behavior.
* Ask questions.
* Make informed decisions.

Our objective is to earn user trust through transparency and responsible development.

---

# 38. Future Security Improvements

As Sipier moves from Beta toward stable releases, we plan to consider improvements such as:

* Official Windows code signing.
* Release checksums.
* Automated dependency scanning.
* Security-focused CI/CD checks.
* Improved release verification.
* Better documentation.
* Security vulnerability reporting.
* More transparent privacy documentation.
* Improved update integrity.
* Reproducible build processes where practical.
* Third-party security review where feasible.

These improvements may be introduced progressively as the project grows.

---

# 39. Final Statement

Sipier is currently a Beta project.

It is a legitimate Windows automation application under active development, but it has not yet reached the level of security assurance expected from mature commercial software.

The current Windows publisher warning is primarily related to the application's ability to establish a verified publisher identity and should not automatically be interpreted as proof of malware.

However, users should always take security warnings seriously.

We will never encourage users to blindly disable their security software or ignore genuine malware detections.

If Windows identifies a specific security threat, investigate the detection before proceeding.

If Windows simply cannot verify the publisher, users who downloaded Sipier from the official release source may independently verify the release and decide whether they trust the application.

Our long-term goal is to make Sipier easier to verify, easier to trust, and safer to distribute.

Until then, we encourage users to stay informed, download only from official sources, keep their security software enabled, and report anything suspicious.

**Transparency is part of security.**

**Sipier — Automate the repetitive. Control the workflow.**

---

## Security Contact

For security-related issues, vulnerabilities, suspicious behavior, or unexpected security detections, please open a security report through the official Sipier GitHub repository.

When reporting an issue, please provide as much technical information as possible without including private or sensitive information.

Thank you for helping us make Sipier safer.

