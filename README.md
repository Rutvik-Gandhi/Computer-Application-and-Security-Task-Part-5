# Computer-Application-and-Security-Task-Part-5

# Network Discovery and Password Cracking Guide

This guide provides step-by-step instructions for network discovery using fping and Nmap, along with password cracking using a chosen tool (Medusa, John, or Hydra).

## 1. fping Sweep

1. **fping Sweep and Target List Generation:**
   - Open a terminal in Kali Linux.
   - Execute the fping command to perform a sweep of the network and generate a target list:
     ```
     fping -a -s -g 192.168.1.0/24
     ```
   - Capture a screenshot showing all alive systems, the generated target list, and the final statistics upon exit.

## 2. Nmap Scan

1. **Nmap Scan with TCP SYN, OS Detection, and Version Detection:**
   - Perform an Nmap scan to discover remote services using the following options:
     - TCP SYN scan (`-sS`): Stealthy scan technique to determine open ports.
     - OS detection (`-O`): Attempts to determine the operating system of the target.
     - Version detection (`-sV`): Attempts to determine service and application versions running on open ports.
     - Verbose output (`-v`): Provides detailed output during the scan.
   - Use the following command:
     ```
     nmap -sS -O -sV -v <target_IP>
     ```
   - Capture screenshots of the Nmap scan output showing the discovery of remote services.

## 3. Password Cracking

1. **Select Open Port and Target IP Address:**
   - From the output of the Nmap scan, select an open port/service running on that port.
   - Provide a screenshot of the target IP address and type of cracking/tool you are attempting to use.

2. **Run Password Cracker:**
   - Choose a password cracker tool (Medusa, John, or Hydra).
   - Use the provided text files to check against a list of users and passwords.
   - Execute the password cracker with the appropriate command and options.
   - Capture screenshots showing the password cracking process and any successful results.

3. **Access the System:**
   - After finding a successful username and password combination, use the information to access the system through the exploited service.
   - Provide a screenshot showing successful access to the system.

## Disclaimer

This guide is for educational purposes only. Ensure that you have proper authorization before performing any network scanning or password cracking activities.
