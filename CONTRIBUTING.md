# Contributing to Sipier

Thank you for your interest in contributing to **Sipier Automation Suite**.

Sipier is an actively developed Windows automation and macro application. Contributions from developers, testers, security researchers, designers, and users are welcome.

Whether you are fixing a bug, improving the user interface, optimizing performance, adding a feature, or improving documentation, your contribution can help make Sipier better.

---

## Table of Contents

* [Before You Contribute](#before-you-contribute)
* [Ways to Contribute](#ways-to-contribute)
* [Getting the Source Code](#getting-the-source-code)
* [Setting Up the Development Environment](#setting-up-the-development-environment)
* [Project Structure](#project-structure)
* [Development Workflow](#development-workflow)
* [Creating a Branch](#creating-a-branch)
* [Making Changes](#making-changes)
* [Testing Your Changes](#testing-your-changes)
* [Submitting a Pull Request](#submitting-a-pull-request)
* [Bug Reports](#bug-reports)
* [Feature Requests](#feature-requests)
* [Security Issues](#security-issues)
* [Code Style](#code-style)
* [Commit Messages](#commit-messages)
* [Documentation Contributions](#documentation-contributions)
* [Pull Request Review](#pull-request-review)
* [What We Look For](#what-we-look-for)
* [What We May Reject](#what-we-may-reject)
* [License](#license)

---

# Before You Contribute

Before making a contribution, please take a moment to:

1. Read the main `README.md`.
2. Read `SETUP_AND_USAGE.md`.
3. Review `APPSAFETY.md`.
4. Check existing GitHub Issues.
5. Check existing Pull Requests.
6. Make sure your contribution does not duplicate existing work.
7. Follow the project's license requirements.

For significant changes, especially major architectural changes or new systems, it is recommended to open an issue first and discuss the proposed approach before starting development.

This helps prevent duplicated work and ensures that contributions fit the direction of the project.

---

# Ways to Contribute

There are many ways to contribute to Sipier.

## Code

You can contribute by:

* Fixing bugs.
* Improving performance.
* Improving stability.
* Adding new automation capabilities.
* Improving macro management.
* Improving the user interface.
* Improving accessibility.
* Improving error handling.
* Improving application architecture.
* Improving Windows compatibility.
* Improving build and release processes.

---

## Bug Reports

If you discover a bug, report it through GitHub Issues.

A good bug report helps developers reproduce and fix the problem quickly.

Include:

* Sipier version.
* Windows version.
* Steps to reproduce the issue.
* Expected behavior.
* Actual behavior.
* Error messages.
* Logs, if available.
* Screenshots or videos when useful.

Please avoid posting sensitive information in public issues.

---

## Feature Requests

Feature suggestions are welcome.

Before creating a feature request, check whether a similar request already exists.

A useful feature request should explain:

* What the feature does.
* Why the feature would be useful.
* What problem it solves.
* How you expect it to work.
* Any relevant examples.

---

## Documentation

Documentation improvements are valuable contributions.

You can help by:

* Fixing spelling mistakes.
* Improving explanations.
* Adding examples.
* Clarifying installation instructions.
* Improving troubleshooting guides.
* Adding developer documentation.
* Translating documentation where appropriate.

---

## Testing

Beta testing is especially valuable for Sipier.

You can contribute by testing:

* New features.
* Macro recording.
* Macro playback.
* Automation reliability.
* Application stability.
* Windows compatibility.
* Installer behavior.
* Performance.
* Edge cases.

If you find unexpected behavior, please report it through GitHub Issues.

---

# Getting the Source Code

Clone the Sipier repository:

```bash
git clone <repository-url>
cd sipier
```

Make sure you are working with the latest available development code before starting new work.

---

# Setting Up the Development Environment

Sipier is currently developed using Python and PyQt6.

Make sure you have:

* Windows 10 or later.
* Python 3.10 or newer.
* pip.
* Git.

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Run Sipier from source:

```bash
python main.py
```

For additional setup information, see:

`SETUP_AND_USAGE.md`

---

# Project Structure

The project currently follows a structure similar to:

```text
sipier/
├── assets/
├── automation/
├── build/
├── dist/
├── theme/
├── ui/
├── main.py
├── build_exe.py
├── requirements.txt
├── Sipier.spec
├── SipierInstaller.nsi
├── README.md
├── SETUP_AND_USAGE.md
├── APPSAFETY.md
├── LICENSE
└── ...
```

### `automation/`

Contains the core automation and macro functionality.

### `ui/`

Contains the application's graphical user interface.

### `theme/`

Contains themes, fonts, styling, and appearance-related systems.

### `assets/`

Contains application resources.

### `main.py`

The main application entry point.

### `build_exe.py`

Build-related utilities for packaging Sipier.

### `Sipier.spec`

PyInstaller configuration.

### `SipierInstaller.nsi`

NSIS installer configuration.

---

# Development Workflow

The recommended contribution workflow is:

1. Fork the repository.
2. Clone your fork locally.
3. Create a dedicated branch.
4. Make your changes.
5. Test your changes.
6. Review your changes.
7. Commit your changes.
8. Push your branch.
9. Open a Pull Request.

Keep changes focused whenever possible.

A Pull Request that fixes one specific bug should generally not include unrelated refactoring unless it is necessary for the fix.

---

# Creating a Branch

Create a new branch before working on changes.

For example:

```bash
git checkout -b fix/macro-playback
```

or:

```bash
git checkout -b feature/advanced-macro-editor
```

Recommended branch naming patterns include:

```text
feature/feature-name
fix/bug-name
refactor/component-name
docs/documentation-name
test/test-name
build/build-change
```

Use a clear and descriptive branch name.

---

# Making Changes

When making changes:

* Keep the implementation focused.
* Avoid unnecessary changes to unrelated files.
* Follow the existing project architecture.
* Avoid introducing unnecessary dependencies.
* Keep code readable.
* Handle errors appropriately.
* Consider Windows compatibility.
* Avoid breaking existing functionality.

If you introduce a new dependency, explain why it is necessary in your Pull Request.

---

# Testing Your Changes

Before submitting a Pull Request, test your changes locally.

At minimum:

1. Run Sipier from source.
2. Test the functionality you changed.
3. Test related functionality that could be affected.
4. Check for errors in the console.
5. Test common edge cases.
6. Verify that existing features still work.

For automation-related changes, test carefully.

Automation bugs can cause unintended actions, so verify:

* Mouse coordinates.
* Keyboard actions.
* Timing.
* Delays.
* Loops.
* Stop mechanisms.
* Unexpected input.

Do not assume that a change works simply because the application launches successfully.

---

# Building the Application

If your changes affect packaging or application startup, test the packaged build as well.

Make sure the application can be successfully packaged using the project's build process.

Pay particular attention to:

* Missing modules.
* Missing assets.
* Missing fonts.
* Theme resources.
* PyInstaller hidden imports.
* Runtime path issues.

A feature that works from Python source but fails in the packaged executable is not considered fully tested.

---

# Submitting a Pull Request

When your changes are ready:

1. Push your branch to your fork.
2. Open a Pull Request against the appropriate Sipier branch.
3. Provide a clear title.
4. Explain what you changed.
5. Explain why you made the change.
6. Describe how you tested it.

A good Pull Request should include:

### Summary

A short explanation of the change.

### Changes

A list of the main modifications.

### Testing

Explain how you tested the changes.

### Screenshots

Include screenshots or recordings when the change affects the UI.

### Additional Notes

Mention anything reviewers should be aware of.

---

# Pull Request Example

A good Pull Request description might look like:

```text
## Summary

Improves macro playback reliability when switching between windows.

## Changes

- Added improved window focus handling.
- Added additional validation before playback.
- Improved error handling.
- Added clearer playback failure messages.

## Testing

Tested on Windows 11.

Tested:
- Basic macro playback
- Window switching
- Multiple macros
- Repeated playback
- Invalid window targets

## Screenshots

Attached to this Pull Request.
```

---

# Bug Reports

Before opening a new bug report:

1. Search existing Issues.
2. Check whether the issue has already been reported.
3. Confirm that you are using the latest version.
4. Try reproducing the issue again.

When reporting a bug, provide as much useful information as possible.

Do not intentionally include:

* Passwords.
* API keys.
* Authentication tokens.
* Private files.
* Personal information.

---

# Feature Requests

Feature requests should focus on solving a real problem or improving the user experience.

When proposing a feature, explain the use case rather than only describing the implementation.

For example:

Instead of:

> Add a new button.

Explain:

> Users currently need to manually recreate frequently used macros. A reusable macro template system would allow users to create and duplicate common workflows more efficiently.

This gives the development team better context for evaluating the proposal.

---

# Security Issues

Security vulnerabilities should not be publicly disclosed before they have been investigated.

If you discover a security issue, follow the security reporting instructions provided in `SECURITY.md`, if available.

Do not use public GitHub Issues to disclose sensitive vulnerability details.

Security reports should include:

* A description of the vulnerability.
* Affected version.
* Steps to reproduce.
* Potential impact.
* Relevant technical details.

Please do not include personal information or sensitive credentials.

---

# Code Style

Keep code consistent with the existing project.

General guidelines:

* Use clear variable and function names.
* Keep functions reasonably focused.
* Avoid unnecessary complexity.
* Add comments when they provide meaningful context.
* Remove unused code.
* Avoid leaving debugging code in Pull Requests.
* Handle exceptions intentionally.
* Avoid silently ignoring errors.
* Keep user-facing error messages understandable.

Do not introduce large architectural changes without discussing them first.

---

# User Interface Contributions

Sipier's interface should remain consistent, clean, and easy to use.

When modifying the UI:

* Maintain visual consistency.
* Avoid unnecessary visual clutter.
* Keep interactions intuitive.
* Consider different window sizes.
* Ensure text remains readable.
* Avoid breaking existing navigation.
* Test animations and transitions for stability.

If you introduce a significant UI change, include screenshots in your Pull Request.

---

# Automation Contributions

Automation functionality requires additional care.

When modifying automation systems:

* Test mouse actions carefully.
* Test keyboard actions carefully.
* Validate coordinates.
* Handle timing correctly.
* Avoid infinite loops.
* Ensure emergency stop mechanisms remain functional.
* Consider unexpected application states.
* Avoid executing actions when the target context is invalid.

Never remove safety mechanisms without a clear replacement.

---

# Dependencies

Avoid adding new dependencies unless they provide meaningful value.

Before adding a dependency:

1. Confirm that the functionality cannot reasonably be implemented using existing dependencies.
2. Check whether the dependency is actively maintained.
3. Check its license.
4. Consider its security history.
5. Consider its impact on application size.
6. Consider whether it works correctly on supported Windows versions.

New dependencies should be documented in the Pull Request.

---

# Commit Messages

Use clear commit messages.

Good examples:

```text
Fix macro playback timing issue
Add emergency stop handling
Improve theme loading
Fix missing font resources
Update installation documentation
Improve error handling for invalid actions
```

Avoid vague messages such as:

```text
update
fix
changes
stuff
test
```

Clear commit messages make the project's history easier to understand.

---

# Documentation Contributions

Documentation is part of the product.

If you change how Sipier works, update the relevant documentation when necessary.

Documentation may include:

* `README.md`
* `SETUP_AND_USAGE.md`
* `APPSAFETY.md`
* `SECURITY.md`
* Other project documentation

Keep documentation accurate and avoid making claims that cannot be verified.

---

# Pull Request Review

All Pull Requests may be reviewed before being merged.

Reviewers may consider:

* Correctness.
* Stability.
* Security.
* Performance.
* Maintainability.
* User experience.
* Compatibility.
* Code quality.
* Documentation.

Reviewers may request changes before a Pull Request is accepted.

Please treat review comments as part of the development process.

---

# What We Look For

Strong contributions generally:

* Solve a clear problem.
* Improve the user experience.
* Are well tested.
* Are easy to understand.
* Follow the existing architecture.
* Avoid unnecessary dependencies.
* Include appropriate documentation.
* Do not introduce security risks.

---

# What We May Reject

A contribution may be rejected if it:

* Introduces unnecessary complexity.
* Breaks existing functionality.
* Creates significant security risks.
* Adds unnecessary dependencies.
* Does not follow project conventions.
* Has insufficient testing.
* Includes unrelated changes.
* Introduces functionality outside the project's intended direction.

A rejected Pull Request does not necessarily mean the idea is bad.

The development team may suggest a different implementation or approach.

---

# Respectful Collaboration

Sipier is intended to be a welcoming project for contributors of different experience levels.

Please:

* Be respectful.
* Be constructive.
* Explain technical disagreements clearly.
* Avoid personal attacks.
* Respect other contributors.
* Focus discussions on the project and its goals.

Contributions are evaluated based on their technical and practical value.

---

# License

By contributing to Sipier, you agree that your contributions may be distributed under the project's license.

Please review the `LICENSE` file before contributing.

If your contribution includes code from another project, ensure that its license permits the intended use and clearly identify the source where required.

Do not submit code that you do not have the legal right to contribute.

---

# Final Notes

Sipier is currently under active development and is still in Beta.

The project architecture, features, and development practices may evolve over time.

We appreciate every contribution, whether it is:

* A bug report.
* A feature suggestion.
* A documentation fix.
* A code contribution.
* A security report.
* A usability improvement.
* A testing report.
* A helpful discussion.

Thank you for helping improve Sipier.

**Sipier — Automate the repetitive. Control the workflow.**
