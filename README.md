# Authenticated vs. Unauthenticated Vulnerability Assessment

## Project Overview

This project evaluates the difference in vulnerability visibility between
authenticated and unauthenticated vulnerability assessments of a Windows 11
virtual machine in Microsoft Azure using Tenable Vulnerability Management.

During testing, three scan states were observed:

1. An unauthenticated assessment with no credentials provided.
2. A credentialed scan attempt in which authentication failed.
3. A successfully authenticated assessment using valid credentials.

The project demonstrates the importance of validating credential status before
interpreting vulnerability scan results.


## Assessment Results

| Assessment | Credential Status | Findings |
|---|---|---:|
| Unauthenticated | No credentials provided | 48 |
| Failed credential attempt | Authentication failed | 48 |
| Authenticated | Valid credentials provided | 80 |

Successful authenticated scanning identified 32 additional findings compared
with the unauthenticated assessment, representing a 67% increase in finding
visibility.

The authenticated assessment also identified an additional High-severity
Windows account configuration issue.


## Key Findings

- Unauthenticated assessment identified 48 findings.
- Providing credentials did not automatically result in successful authentication.
- Credential status validation identified a failed authentication attempt.
- Successful authenticated scanning identified 80 findings.
- Authenticated scanning increased finding visibility by approximately 67%.
- The authenticated assessment identified an additional High-severity Windows
  account configuration issue.
- Credentialed scanning provided additional host-level Windows information
  unavailable through the unauthenticated assessment.


  
