# CIP-B105 Case Study 3 – Illegal File Transferring

## Overview

This repository contains my submission for CIP-B105 Case Study 3. The investigation involved examining a Windows 7 memory image to determine whether the available evidence supported an alleged illegal file transfer.

The analysis focused on identifying the relevant user account, examining the suspect system, reviewing network and process activity, recovering command activity, and correlating USB and user artefacts. The final stage brought the different findings together into a single timeline.

## Investigation Coverage

The assessment covered Lessons 14–21 and included:

- Memory evidence preparation and preservation
- User account and SID identification
- System and hardware identification
- Network and process analysis
- Command history examination
- USB storage and drive-letter analysis
- User-specific MountPoints2 examination
- Internet and Shellbag activity
- Timeline reconstruction and evidence correlation

## Tools Used

The investigation was mainly carried out in Kali Linux using:

- Volatility 2.6.1
- Python 2
- `strings`
- `grep`
- `tee`
- Standard Linux file and hashing utilities

Volatility plugins were used to examine processes, network connections, Registry data, command activity, user accounts and other artefacts preserved in memory.

## Key Findings

The investigation identified the IEUser account as relevant to the examined activity. Registry and memory artefacts were used to establish the suspect system environment and examine the presence of removable storage.

USB-related Registry evidence showed that a USB storage device had been attached to the system. User-specific artefacts also supported interaction with a mounted volume. Shellbag evidence showed activity involving the Downloads folder.

Network, browser, command and USB evidence were considered together rather than relying on a single artefact. This allowed the final conclusions to be based on corroborated evidence while recognising the limitations of a memory-only investigation.

## Repository Contents

The submission archive contains the final report and supporting investigation material produced during the assessment. This includes saved command output, supporting reports, screenshots, recovered artefacts where applicable, and the commands used during the investigation.

## Evidence Handling

A working copy of the supplied memory image was used during the investigation. Hashing and evidence-preservation procedures were followed to maintain integrity.

The original evidence image is not included in this repository. This avoids unnecessary redistribution of the assessment evidence.

## Limitations

The findings are based on the artefacts available within the acquired memory image. Memory represents a particular point in time, so some historical activity may no longer have been resident when the image was captured.

Individual artefacts were therefore interpreted cautiously and correlated with other evidence before conclusions were reached.

## Author

**Asmau Danzaria**  
CIP-B105 – Case Study 3  
Digital Forensics Investigation
