# Linux QA

## What is it?
Linux QA is a utility to audit fresh linux(RHEL/Oracle Linux) installation per Organization's recommended standards.

## Documentation
This utility is a bash script that checks for various configuration on the system. While execution this utility creates a temporary file under /tmp. The output file generated is in PDF format. The system performs following checks:
        1     OS, Release, and Kernel Version
        2     File System Information
        3     Volume Groups
        4     Logical Volumes
        5     SNMP Configuration
        6     Repository Registration Status
        7     Pending Patches
        8     Services List
        9     NTP Configuration
       10     Sendmail Configuration
       11     User Accounts
       12     BMC Patrol Configuration
       13     Tivoli TSM Configuration

Following are the important elements of this utility:

  - bin: Directory where all the executables are located
  - log: directory where the execution log are stored
  - out: Directory where PDF report is generated
  - log4bash.conf: A file using which log output can be tuned (for debuggin purposes)
  - text2pdf: A utility that converts a text file into PDF.
  - qa: Linux Audit utility.

## Installation
 - Copy the whole linuxqa directory on the machine to be audited (suggested place /root/linuxqa)
 - Change directory to linuxqa/bin
```
  # cd <install_dir>/linuxqa/bin
```
 - Run qa
```
  # ./qa
```
 - For Help run
```
  # ./qa -h
```

