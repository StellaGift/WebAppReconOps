# Web Application Scanning and Enumeration Script

## Overview

This Bash script is designed to facilitate the scanning and enumeration of web applications by providing a simple menu-based interface to choose from various tools. The script allows users to perform scans using Nmap, Nikto, Dirb, or Enum4linux individually or simultaneously with four different terminals.

## Prerequisites

- Nmap: Network exploration tool and security scanner (https://nmap.org/)
- Nikto: Web server scanner (https://cirt.net/Nikto2)
- Dirb: URL bruteforcing tool (https://tools.kali.org/web-applications/dirb)
- Enum4linux: Information gathering tool for Windows and Samba systems (https://tools.kali.org/information-gathering/enum4linux)

Make sure these tools are installed and available in your system's PATH before using the script.

## Usage

1. Save the script in a file with a `.sh` extension, for example, `web_scan.sh`.
2. Make the script executable: `chmod +x web_scan.sh`
3. Run the script: `./web_scan.sh`

Follow the on-screen prompts to select the scanning tool and provide the target IP address when prompted.

## Options

1. **Nmap Scan**
   - Performs a comprehensive Nmap scan on the specified target IP.
   - Options used: `-p1-65535 -sV -sS -T4 -A -O -oA (an output file is predefined and a file named nmap_scan_results specified. Nmap scan result will save in all three extensions).`

2. **Nikto Scan**
   - Runs Nikto to scan the specified target IP for potential vulnerabilities.
   - Options used: `-h`

3. **Dirb Scan**
   - Utilizes Dirb to perform URL bruteforcing on the target IP.
   - Options used: `http://`

4. **Enum4linux Scan**
   - Executes Enum4linux to gather information on Windows and Samba systems.
   - Options used: None

## Example

```bash
./web_scan.sh
```

Follow the prompts to select a scanning tool, and the Nmap scan will automatically save its results to files without prompting for a filename. The chosen tool will execute with the specified parameters.

## Note

- Ensure that the selected scanning tools are installed and accessible in the system's PATH.
- The script will exit after completing the chosen scan.

- Script is highly scalable and modifiable based on needs.

**Disclaimer: Use this script responsibly and only on systems where you have explicit permission for scanning. Unauthorized scanning may violate ethical and legal standards. Stella GIft is not responsible for any misuse or consequences arising from the use of this script.**
