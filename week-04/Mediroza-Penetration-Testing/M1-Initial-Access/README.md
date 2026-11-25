# M1 - Initial Access

## Objective

Investigate the authorised project target and document findings related to the initial access milestone.

## Target

https://medirozahospital.com

## Project Details

- Client: Mediroza General Hospital
- Project: Networkwalks Penetration Testing
- Batch: B083
- Milestone: M1 - Initial Access
- Testing Type: Black-box Web Application Penetration Testing

## Activities

- Public website reconnaissance
- Identification of publicly accessible entry points
- Review of patient and staff login pages
- HTTP response header inspection
- TLS certificate and connection inspection
- Session cookie configuration review
- Inspection of publicly available website resources
- Documentation of observed security configurations

## Initial Observations

### 1. Public Website

The homepage contains navigation links for:

- Home
- About
- Doctors
- Contact
- Patient Portal

The website also provides a Staff Login link.

### 2. Login Pages

The following login pages were identified:

- Patient Portal: `/patient/login.php`
- Staff Login: `/staff/login.php`

Observations:

- Both login pages returned HTTP 200 OK.
- Both forms use the POST method.
- Both forms submit to `login.php`.
- Username and password input fields were identified.
- No credentials were entered.

### 3. TLS Configuration

The following observations were recorded:

- HTTPS connection observed.
- TLS 1.3 observed.
- Certificate reported as valid and trusted.
- Certificate expiry: 1 March 2027.

### 4. HTTP Response Headers

The following security headers were not observed in the captured homepage, Patient Portal and Staff Login responses:

- Strict-Transport-Security
- Content-Security-Policy
- X-Frame-Options
- X-Content-Type-Options
- Referrer-Policy
- Permissions-Policy

These are preliminary configuration observations, not confirmed exploitable vulnerabilities.

### 5. Technology Disclosure

The Patient Portal and Staff Login responses exposed:

- Web server: LiteSpeed
- PHP version: PHP/8.2.36

These details provide technology information but do not independently establish a vulnerability.

### 6. Session Cookie Observations

The observed PHPSESSID cookie had the following attributes:

| Attribute | Observation |
|---|---|
| Secure | Enabled |
| HttpOnly | Not enabled |
| SameSite | Not specified |
| Path | / |
| Expiry | Session |

The session identifier remained unchanged after a page refresh.

This limited observation does not establish a session fixation vulnerability.

### 7. Login Form Inspection

The Patient Portal form contained:

- Username input
- Password input
- Show-password checkbox
- Sign-in button

Additional observations:

- `autocomplete="off"` was present on username and password fields.
- No hidden input fields were identified in the inspected form.
- No visible CSRF token was identified in the inspected form markup.
- No client-side `required` attributes were observed.

These observations alone do not establish authentication or CSRF vulnerabilities.

### 8. Publicly Available Website Resources

The following resources were inspected:

- `robots.txt`
- `sitemap.xml`
- `styles.css`

The sitemap listed four public pages:

- `index.html`
- `about.html`
- `doctors.html`
- `contact.html`

The inspected homepage source did not contain visible JavaScript script tags or `/api/` references.

The stylesheet contained presentation rules for the website, authentication pages and patient portal interface.

No sensitive configuration or credentials were identified in the inspected stylesheet.

## Evidence

Screenshots are stored in the Evidence folder.

Evidence includes:

- Homepage screenshot
- About page screenshot
- Doctors page screenshot
- Contact page screenshot
- Patient Portal login page
- Staff Login page
- Homepage response headers
- Patient Portal response headers
- Staff Login response headers
- TLS certificate details
- TLS connection details
- Session cookie attributes
- Patient login form inspection
- Staff login form inspection
- Login response observations
- Robots.txt
- Sitemap.xml
- Stylesheet inspection

Sensitive session values and personal information must be redacted before publishing or sharing evidence.

## Testing Limitations

- The shared Week 4 Google Drive folder currently contains only the project guidance PDF.
- The three sample patient PDF reports required for M1 have not been located in the shared folder.
- Authenticated portal access has not been tested.
- Successful initial access has not been demonstrated.
- The three PDF reports have not been retrieved.
- Further testing requiring additional project files is pending clarification from the mentor.

## Scope Clarification

The mentor instructed participants:

- Do not download or access database backups.
- Do not access files outside the explicitly authorised project scope.

All further testing must follow these instructions.

## Safety

- Follow the authorised project scope.
- Do not access or disclose genuine patient records.
- Do not perform destructive testing.
- Do not attempt unauthorised authentication.
- Stop if genuine confidential information is encountered.
- Redact sensitive information from evidence before sharing.

## Status

Reconnaissance documented.

M1 initial access testing remains pending authorised sample files and clarification from the mentor.