# Setup Instructions

## Prerequisites
Before you begin, ensure you have met the following requirements:
* You have a `Windows/Linux/Mac` machine.
* You have installed the latest version of `Python`.
* You have installed `Nmap`, `OpenVAS`, and `Wireshark`.

## Tool Installation

### Installing Nmap
#### Windows:
- Download the latest version of Nmap from [https://nmap.org/download.html](https://nmap.org/download.html)
- Run the installer and follow the on-screen instructions.

#### Linux:
- Use your distribution's package manager, e.g., for Ubuntu/Debian:
  ```bash
  sudo apt-get install nmap
  
### Installing OpenVAS (GVM)
- **Linux**: OpenVAS is best supported on Linux. Install it on Ubuntu/Debian with the following commands:
  ```bash
  sudo apt-get install gvm
  sudo gvm-setup
  sudo gvm-start

  # System Setup Instructions

## OpenVAS on Windows and Mac
- **Recommendation:** Use a virtual machine running a Linux distribution since OpenVAS does not natively support Windows or Mac OS.

## Installing Wireshark
- **Windows:**
  1. Download the installer from [Wireshark's website](https://www.wireshark.org/download.html).
  2. Run the installer using the default options.
- **Linux (Ubuntu/Debian):**
  1. Execute `sudo apt-get install wireshark`.
  2. During installation, select 'Yes' to allow non-superusers to capture packets.
- **Mac:**
  1. Install Wireshark using Homebrew: `brew install --cask wireshark`.

## Python Environment Setup
1. Install Python from the [official Python website](https://www.python.org/downloads/) or use your operating system's package manager.
2. Ensure `pip` is installed by running `python -m ensurepip --upgrade`.
3. Optionally, set up a virtual environment:
   +++bash
   python -m venv venv
   source venv/bin/activate # For Linux/Mac
   venv\Scripts\activate # For Windows
   +++

## Additional Dependencies
- Install required Python libraries by executing `pip install -r requirements.txt`.
- Ensure you have a `requirements.txt` file in your repository listing all dependencies.

## Configuration
- **Nmap:**
  - Set up a default scan profile or target list as needed.
- **OpenVAS:**
  - Sync the vulnerability definitions: `sudo gvm-feed-update`.
- **Wireshark:**
  - Configure capture filters or customize the interface list as required for your project.

**Note:** Replace any placeholders with actual commands or links relevant to your project. Verify that the commands are current with the latest versions of the tools. It is crucial to test these setup instructions on a clean environment to ensure they work as expected.
