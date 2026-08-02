# Sipier — Setup and Usage Guide

This guide explains how to install, configure, run, and use Sipier.

---

# 1. Installation

## For Regular Users

If you downloaded Sipier from the official release:

1. Download the latest Sipier installer.
2. Run the installer.
3. Follow the installation instructions.

<img width="493" height="383" alt="{CC0DF485-FA41-4D8C-970F-BCC646C79E9C}" src="https://github.com/user-attachments/assets/16268b83-4172-4cee-a168-2c698e8c2792" />


4. Launch Sipier from the Start Menu or desktop shortcut.

<img width="249" height="56" alt="{3098C325-D504-435A-879D-C0FBED3B8275}" src="https://github.com/user-attachments/assets/0dfd32f4-7e94-478d-ab4d-937955c78f7b" />


5. Start creating and running your automation macros.

<img width="1090" height="745" alt="{6FC09111-2A0B-48C6-B7EE-ED98972FD1BB}" src="https://github.com/user-attachments/assets/b8d80981-84fb-46d1-bd22-e1bc701b072a" />

The packaged version of Sipier includes the required application runtime and dependencies.

You do **not** need to manually install Python or PyQt6 to use the packaged application.

---

# 2. Running Sipier from Source

This section is intended for developers who want to run Sipier directly from the source code.

## Requirements

Before running Sipier from source, make sure you have:

* Windows 10 or later
* Python 3.10 or newer
* pip
* Git

## Clone the Repository

Clone the repository and enter the project directory:

```bash
git clone <repository-url>
cd sipier
```

## Install Dependencies

Install the required Python packages:

```bash
pip install -r requirements.txt
```

## Start Sipier

Run the main application:

```bash
python main.py
```

If the application starts successfully, the Sipier interface should appear.

---

# 3. Understanding the Project

The main project structure is:

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
└── SipierInstaller.nsi
```

### `main.py`

The main entry point of the application.

### `automation/`

Contains the core automation systems responsible for executing macros and automated actions.

### `ui/`

Contains the graphical user interface and application screens.

### `theme/`

Contains theme management, visual styles, fonts, and related appearance systems.

### `assets/`

Contains application resources used by the interface.

### `build_exe.py`

Build utility used to package Sipier into a Windows executable.

### `Sipier.spec`

PyInstaller configuration used during the executable build process.

### `SipierInstaller.nsi`

NSIS configuration used to create the Windows installer.

---

# 4. Creating Your First Macro

Launch Sipier and open the macro or automation workspace.

Create a new macro and give it a recognizable name.

Add the actions you want Sipier to perform.

Depending on the available automation features, actions may include:

* Mouse clicks
* Mouse movement
* Keyboard input
* Delays
* Action sequences
* Repeated actions
* Loops

Configure each action according to your requirements.

Save the macro when finished.

---

# 5. Recording a Macro

If macro recording is available:

1. Open the macro recorder.
2. Start recording.
3. Perform the mouse and keyboard actions you want to automate.
4. Stop the recording.
5. Review the recorded actions.
6. Edit or adjust the sequence if necessary.
7. Save the macro.

Recorded macros can then be replayed whenever required.

---

# 6. Running a Macro

To run an existing macro:

1. Open your saved macros.
2. Select the macro you want to execute.
3. Review the configured actions.
4. Start playback.
5. Sipier will execute the actions in sequence.

Make sure the target application or window is ready before starting the macro.

---

# 7. Stopping Automation

Always keep the emergency stop functionality accessible while running automation.

If a macro behaves unexpectedly or you need to stop execution immediately, use the configured emergency stop method.

Do not leave unattended automation running unless you are confident that the macro is behaving correctly.

---

# 8. Editing a Macro

Open an existing macro to modify its automation sequence.

You can adjust available settings such as:

* Action order
* Mouse positions
* Keyboard inputs
* Delays
* Repetition counts
* Loop behavior

After making changes, save the macro before running it again.

---

# 9. Building Sipier

Developers can create a distributable Windows build using the project's build configuration.

Install the required dependencies first:

```bash
pip install -r requirements.txt
```

Then run the project's build process:

```bash
python build_exe.py
```

The generated executable files will be placed in the configured build or distribution directory.

The exact output location may depend on the current PyInstaller configuration.

---

# 10. Creating the Windows Installer

Sipier uses NSIS for creating the Windows installer.

Make sure NSIS is installed on the development machine.

Open:

```text
SipierInstaller.nsi
```

in the NSIS compiler and build the installer.

The resulting installer can be distributed to users as the standard installation package for Sipier.

---

# 11. Troubleshooting

## Sipier Does Not Start

Check that:

* You are using a supported version of Windows.
* All required dependencies are installed.
* You are running the correct Python version.
* The project is being launched from the correct directory.

If running from source, reinstall dependencies:

```bash
pip install -r requirements.txt
```

---

## Module Not Found Errors

If Python reports an error such as:

```text
ModuleNotFoundError
```

make sure you are running Sipier from the project root directory.

For example:

```text
sipier/
├── main.py
├── theme/
├── ui/
└── automation/
```

Run the application from the directory containing `main.py`.

---

## Macro Does Not Execute Correctly

Check the following:

* The target application is open.
* The target window is in the expected position.
* Mouse coordinates are correct.
* Delays are long enough for the target application to respond.
* The macro actions are in the correct order.
* The target application has not changed its interface.

Try running the macro manually while observing each action.

---

## Application Behaves Unexpectedly

Stop the macro immediately using the emergency stop functionality.

Review the macro configuration and check for incorrect coordinates, timing values, loops, or action sequences.

If the issue persists, create a GitHub issue with reproduction steps and relevant logs.

---

# 12. Best Practices

For reliable automation:

* Use reasonable delays between actions.
* Test new macros before running them unattended.
* Keep macros organized and clearly named.
* Avoid unnecessary loops.
* Verify mouse coordinates before playback.
* Always know how to trigger the emergency stop.
* Test automation after changes to the target application.

---

# 13. Safety and Responsible Use

Sipier is intended for legitimate automation, productivity, testing, and repetitive workflow tasks.

Users are responsible for ensuring that their use of Sipier complies with the rules, terms of service, and policies of any software, website, game, or service they interact with.

Do not use Sipier to perform actions that violate applicable laws, regulations, or third-party terms of service.

---

# 14. Getting Help

If you encounter a problem:

1. Check this guide.
2. Check the project's GitHub issues.
3. Search for an existing issue.
4. Open a new issue if the problem has not already been reported.

When reporting a problem, include:

* Sipier version
* Windows version
* Steps to reproduce the issue
* Expected behavior
* Actual behavior
* Error messages
* Relevant logs
* Screenshots when helpful

Providing detailed information helps the development team diagnose and resolve issues faster.

---

**Sipier — Automate the repetitive. Control the workflow. Save time.**
