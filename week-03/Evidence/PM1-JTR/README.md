# PM1 – Password Cracking with John the Ripper

## Objective
To extract the password hash from a locked PDF and recover its password using John the Ripper.

## Tools Used
- John the Ripper 1.9.0 Jumbo
- Johnny GUI
- Strawberry Perl
- pdf2john.pl

## Procedure
1. Installed John the Ripper and Johnny.
2. Configured Johnny to detect the John executable.
3. Installed Strawberry Perl to execute the PDF hash extraction script.
4. Used `pdf2john.pl` to extract the PDF password hash.
5. Saved the extracted hash in a text file.
6. Loaded the hash into Johnny.
7. Started the password-cracking process.
8. Successfully recovered the PDF password.
9. Verified the password by opening the locked PDF.

## Result
**Status:** Successfully completed.

**Recovered password:** `GOOD-LUCK`

## Evidence
- `W3-PM1-PDF1-UNLOCKED.png`
- `W3-PM1-hash.txt`

## Learning Outcome
Learned PDF hash extraction, John the Ripper configuration, Perl script execution, and password recovery using Johnny.

## Disclaimer
This activity was performed on the provided internship lab PDF for educational purposes.
