# Authenticated vs. Unauthenticated Vulnerability Assessment

## Project Overview

This project compares authenticated and unauthenticated vulnerability
assessments of a Windows 11 virtual machine using Tenable Vulnerability
Management.

The objective was to evaluate how credentialed access affects vulnerability
visibility and the amount of host-level information available to the scanner.

## Environment

- Tenable Vulnerability Management
- Microsoft Azure
- Windows 11 Virtual Machine
- Network Security Groups (NSG)

## Assessment Results

| Assessment | Credential Status | Findings |
|---|---|---:|
| Unauthenticated | No credentials provided | 46 |
<img width="632" height="842" alt="august 28 (2)" src="https://github.com/user-attachments/assets/1f3c29d6-c600-42cc-b749-c459883a265d" />
<img width="603" height="328" alt="august 28 (3)" src="https://github.com/user-attachments/assets/01faf2da-2772-4653-823e-049eadef0fc0" />

| Authenticated | Valid credentials provided | 79 |
<img width="652" height="410" alt="august 28 (1)" src="https://github.com/user-attachments/assets/4d27ff31-0797-4961-84e9-615fc1d2bf13" />
<img width="608" height="845" alt="august 28" src="https://github.com/user-attachments/assets/ce874c4b-875c-4838-9e3f-3dc62593b100" />


Authenticated scanning identified 33 additional findings, representing
approximately a 72% increase in finding visibility.

## Key Findings

The authenticated assessment provided substantially greater host-level
visibility, including Windows user information, password policy, WMI data,
process information, network interfaces, system information, and other
configuration details unavailable through the unauthenticated assessment.

Both assessments identified the same four Medium-severity findings and one
Low-severity finding.

## Assessment Limitations

Although Tenable confirmed valid credentials, the authenticated assessment
reported that OS security patch assessment failed and that the scanner could
not access the Windows Registry.

This demonstrates that successful authentication should not automatically
be interpreted as complete assessment coverage. Credential status and scan
quality should be validated when reviewing vulnerability results.

## Skills Demonstrated

Tenable Vulnerability Management • Vulnerability Assessment •
Authenticated Scanning • Vulnerability Analysis • Scan Validation •
Microsoft Azure • Windows 11
