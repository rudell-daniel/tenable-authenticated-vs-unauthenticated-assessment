# tenable-authenticated-vs-unauthenticated-assessment
Comparative vulnerability assessment demonstrating the visibility differences between authenticated and unauthenticated Tenable scanning of a Windows 11 Azure VM.
# Authenticated vs. Unauthenticated Vulnerability Assessment

## Project Overview

This project compares authenticated and unauthenticated vulnerability
assessments of a Windows 11 virtual machine hosted in Microsoft Azure
using Tenable Vulnerability Management.

## Objective

Evaluate how credentialed access affects vulnerability visibility and
determine whether authenticated scanning identifies security exposures
not detected through unauthenticated assessment.

## Environment

- Tenable Vulnerability Management
- Microsoft Azure
- Windows 11 Virtual Machine

## Assessment Methodology

1. Configured the Windows 11 Azure VM as the assessment target.
2. Performed an unauthenticated vulnerability assessment.
3. Performed an authenticated vulnerability assessment using valid credentials.
4. Compared findings from both assessments.
5. Reviewed differences in vulnerability visibility and severity.

## Results

| Assessment | Findings |
|---|---:|
| Unauthenticated | 48 |
| Authenticated | 80 |

Authenticated scanning identified 32 additional findings, representing
a 67% increase in finding visibility.

The credentialed assessment also identified an additional High-severity
Windows account configuration issue that was not identified during the
unauthenticated assessment.

## Key Takeaway

The assessment demonstrated how authenticated scanning can provide
deeper visibility into host-level configurations and vulnerabilities
than unauthenticated network-based assessment alone.

## Skills Demonstrated

Tenable Vulnerability Management • Vulnerability Assessment •
Credentialed Scanning • Finding Analysis • Risk Prioritization •
Microsoft Azure
