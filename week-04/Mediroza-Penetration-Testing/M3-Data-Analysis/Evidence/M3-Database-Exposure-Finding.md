\# M3 - Database Exposure Finding



\## Finding

Publicly accessible database backup



\## Location

/old/mediroza\_db\_backup\_2019.sql



\## Evidence

\- Public directory listing

\- Database name: mediroza\_hr

\- 30 staff records

\- 10 shareholder records

\- Salary and ownership information exposed



\## Impact

Confidential employee and shareholder information

was accessible without authentication.



\## Preliminary Severity

High



\## Recommended Remediation

\- Remove public access to database backups.

\- Store backups outside the web root.

\- Disable directory listing.

\- Review access logs and rotate exposed credentials if any.



\## Additional Observations



\- Backup filename: mediroza\_db\_backup\_2019.sql

\- Backup date in SQL comments: 2019-08-27

\- Web server Last Modified date: 2026-09-04

\- CMS identified: Mediroza CMS 1.4.2

\- Database: mediroza\_hr



The difference between the backup date and

the server modification date requires further

verification.

