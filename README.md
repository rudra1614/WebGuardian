
# 🛡️ WebGuardian
**The Multi-Tool Web Vulnerability Scanner**

WebGuardian is an automated security scanning tool that streamlines the process of web vulnerability assessment by leveraging multiple Linux security tools and custom scripts. This powerful Python-based scanner helps security professionals and penetration testers identify vulnerabilities in web applications efficiently.

## 📋 Overview

WebGuardian v1.2 automates the tedious process of running multiple security scanners against a target domain, aggregating results, and presenting them in a user-friendly format. It's designed to save time during security assessments and provide comprehensive vulnerability detection.

![image](https://github.com/user-attachments/assets/c945bbd5-85b7-4f36-aaf5-7409d5c1c97d)



## ✨ Features

- 🔍 **Multi-Tool Integration**: Utilizes various security scanning tools including dmitry, theHarvester, and more
- 🎯 **Automated Scanning**: Single command execution for comprehensive security assessment
- ⏱️ **Real-time Progress Tracking**: Built-in spinner/loader with scan time tracking
- 🎨 **Colored Output**: Easy-to-read vulnerability reports with color-coded severity levels
- ⚙️ **Flexible Configuration**: Skip specific tests or disable UI elements as needed
- 🛑 **Interactive Control**: Ability to skip tests or quit gracefully with keyboard shortcuts
- 📊 **Vulnerability Classification**: Automatic severity rating and remediation suggestions

## 🚀 Installation

### Prerequisites

- Python 3.x
- Linux operating system
- Internet connectivity
- Required security tools (dmitry, theHarvester, etc.)

### Setup

1. Clone the repository:
```bash
git clone https://github.com/rudra1614/WebGuardian.git
cd WebGuardian
```

2. Make the script executable:
```bash
chmod +x webguardian.py
```

3. Ensure all required security tools are installed on your system

## 💻 Usage

### Basic Scan

Scan a target domain:
```bash
python3 webguardian.py example.com
```

### Advanced Options

Skip specific tests:
```bash
python3 webguardian.py example.com --skip dmitry --skip theHarvester
```

Disable the spinner/loader:
```bash
python3 webguardian.py example.com --nospinner
```

Update WebGuardian to the latest version:
```bash
python3 webguardian.py --update
```

Display help information:
```bash
python3 webguardian.py --help
```

## ⌨️ Interactive Controls

While scanning:
- **Ctrl+C**: Skip the current test
- **Ctrl+Z**: Quit WebGuardian

## 📊 Scan Process Indicators

WebGuardian provides time estimates for each scan:
- **[HIGH]**: Scan may take longer (unpredictable duration)
- **[MEDIUM]**: Scan may take less than 10 minutes
- **[LOW]**: Scan may take less than a minute or two

## 🔐 Vulnerability Severity Levels

Results are classified by severity:
- **CRITICAL**: Requires immediate attention - may lead to compromise or service unavailability
- **HIGH**: May not lead to immediate compromise, but has considerable probability
- **MEDIUM**: Multiple vulnerabilities may be correlated for sophisticated attacks
- **LOW**: Not serious, but recommended to address
- **INFO**: Informational findings for consideration

## 🏗️ Project Structure

```
WebGuardian/
├── webguardian.py    # Main scanner script
└── README.md         # Project documentation
```

## 🛠️ Technical Details

- **Language**: Python 3
- **Main Dependencies**: 
  - `argparse` - Command-line parsing
  - `subprocess` - External tool execution
  - `threading` - Concurrent scanning operations
  - `urllib` - URL parsing and validation

## ⚠️ Legal Disclaimer

**IMPORTANT**: WebGuardian is intended for authorized security testing only. Users must:
- Obtain proper authorization before scanning any systems
- Comply with all applicable laws and regulations
- Use this tool responsibly and ethically

Unauthorized access to computer systems is illegal. The developers assume no liability for misuse of this tool.

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests
- Improve documentation

## 📝 License

This project is currently unlicensed. Please contact the repository owner for usage permissions.

## 👤 Author

**Rudra** ([rudra1614](https://github.com/rudra1614))

## 📞 Support

For issues, questions, or suggestions:
- Open an issue on GitHub
- Contact the repository maintainer

## 🔄 Version History

- **v1.2** - Current stable release
  - Multi-tool integration
  - Enhanced user interface
  - Improved vulnerability classification

---

**⚡ Quick Start**: `python3 webguardian.py example.com`

*Remember: Always obtain proper authorization before conducting security assessments.*
