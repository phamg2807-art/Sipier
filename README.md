# Sipier
Sipier is a modern Windows automation and macro tool built to simplify repetitive tasks. Record and replay mouse and keyboard actions, create custom automation workflows, and control every step with precision through a clean, intuitive interface.

**Modern Windows automation and macro software designed to simplify repetitive tasks.**

Sipier is a desktop automation application built with Python and PyQt6. It allows users to create, record, manage, and execute automated mouse and keyboard workflows through a clean and intuitive interface.

Whether you need to automate repetitive actions, create custom macros, or streamline everyday workflows, Sipier provides powerful automation tools without requiring users to write scripts or understand programming.


<img width="1103" height="747" alt="{ADFD9095-A7C1-4CDE-B713-3F15A6F9B621}" src="https://github.com/user-attachments/assets/351abac7-f302-4b25-8af1-564df0e14420" />


<img width="1092" height="742" alt="{46189E9C-D581-40F1-979A-DCF69D7F9D39}" src="https://github.com/user-attachments/assets/29b84729-b4bc-45bf-b239-02936e3e5e61" />


<img width="1092" height="742" alt="{857DFDAE-C0BF-4442-AED4-13FA88473311}" src="https://github.com/user-attachments/assets/835641ce-9b1f-4efc-a158-cd85e1774e58" />



---
## 📖 Documentation & Guides

* 🚀 [Click here to read the Setup and Usage Guide](./SETUP_AND_USAGE.md)


## Features

* Mouse and keyboard automation
* Macro recording and playback
* Custom automation workflows
* Configurable action sequences
* Adjustable delays and timing
* Macro management
* Loop and repetition support
* Emergency stop controls
* Modern PyQt6 desktop interface
* Windows executable and installer
* Lightweight and easy-to-use experience

---

## Installation

### For Users

Download the latest version from the **GitHub Releases** section.

Run the Sipier installer and follow the installation instructions.

The packaged application includes the required runtime dependencies, so users do not need to install Python or PyQt6 separately.

### For Developers

Clone the repository:

```bash
git clone <repository-url>
cd sipier
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Run Sipier from source:

```bash
python main.py
```

---

## Usage

### Creating Automation

Create a new macro and configure the actions you want Sipier to perform.

### Recording Actions

Use the recording functionality to capture mouse and keyboard interactions and convert them into a reusable automation sequence.

### Running Macros

Select a saved macro and start playback. Sipier will execute the configured actions according to the selected settings.

### Managing Macros

Create, edit, organize, and reuse your automation workflows from within Sipier.

---

## Project Structure

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

### Main Components

* `automation/` — Core automation and macro functionality
* `ui/` — Application interface and user interaction
* `theme/` — Theme management, fonts, and visual styling
* `assets/` — Application resources
* `main.py` — Application entry point
* `build_exe.py` — Executable build process
* `Sipier.spec` — PyInstaller configuration
* `SipierInstaller.nsi` — Windows installer configuration

---

## Technology Stack

* **Python** — Core application language
* **PyQt6** — Desktop user interface
* **PyInstaller** — Application packaging
* **NSIS** — Windows installer creation

---

## Building from Source

To build the Windows executable, make sure the required dependencies are installed and run the project's build process.

The resulting application can then be packaged using the provided installer configuration.

For development, running Sipier directly from the Python source is recommended.

For distribution, the packaged executable and installer should be used instead of requiring end users to install Python dependencies manually.

---

## Roadmap

Future development may include:

* Advanced macro editing
* More automation action types
* Improved macro recording
* Enhanced workflow management
* Smart automation features
* Better error handling and diagnostics
* Expanded customization options
* Performance improvements
* Additional Windows integration
* Improved accessibility and usability

The roadmap may change as Sipier continues to evolve.

---

## Contributing

Contributions, suggestions, and feedback are welcome.

If you would like to contribute:

1. Fork the repository.
2. Create a new branch for your changes.
3. Make your improvements.
4. Test your changes thoroughly.
5. Submit a pull request with a clear description of your changes.

Please keep contributions focused, well-structured, and consistent with the existing project architecture.

---

## Bug Reports and Feature Requests

Found a bug or have an idea for Sipier?

Open an issue on GitHub and provide as much relevant information as possible, including:

* A description of the issue
* Steps to reproduce the problem
* Expected behavior
* Actual behavior
* Operating system information
* Relevant screenshots or logs

Feature requests are also welcome.

---

## License

This project is currently distributed under the license specified in the repository.

Please review the project's license file for information about usage, modification, and redistribution.

---

## Status

Sipier is actively being developed.

Features, architecture, and functionality may change as the project evolves.

---

**Sipier — Automate the repetitive. Control the workflow. Save time.**
