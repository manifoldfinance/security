# Vulnerability Disclosure Policy

Security is core to our values, and we appreciate the input of security
researchers acting in good-faith to help us maintain a high standard for the
security and privacy of our users, which includes encouraging responsible
vulnerability research and disclosure. This policy sets out our definition of
good-faith in the context of finding and reporting vulnerabilities, as well as
what you can expect from us in return.

## Encrypted Communication Methods

Public Key Info for `sam@manifoldfinance.com`
Public Fingerprint:

```console
EA82 E243 8E63 F4BD C4AB F453 F773 F8D6 A1A6 D802. 
```
This Fingerprint is unique to your public key. Share this so that your contacts can verify that they have the right key to encrypt for.

[Encrypted Contact Page](https://flowcrypt.com/me/sammanifoldfinance)     
[Public PGP Key](https://flowcrypt.com/pub/sam@manifoldfinance.com)

FlowCrypt also provides an Attestation service, you can access that here: [https://flowcrypt.com/attester/](https://flowcrypt.com/attester/)

### Defects and Reporting Information

[see https://github.com/manifoldfinance/pki#security-bug-handling-process](https://github.com/manifoldfinance/pki#security-bug-handling-process)


## Expectations

When working with us, according to this policy, you can expect us to:

- Extend Safe Harbor for your vulnerability research that is related to this
  policy;
- Work with you to understand and validate your report, including a timely
  initial response to the submission; and
- Work to remediate discovered vulnerabilities in a timely manner.

## Official Channels

Any vulnerability deemed to be in-scope, according to this policy, should be
reported directly to this program through the Encrypted Communciations Methods listed above.
All communications between the researcher and program team regarding any reported
vulnerability should be confined to the comments section of the corresponding
report.

## Awards

| Severity | Description                                                             | Examples                                                                                                 |
| -------- | ----------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| Critical | Systemic compromise                                                     | XXE Injection and SQL Injection with significant impact; <br/>RCE and Vertical Authentication Bypass.    |
| High     | Full access to other user's private data                                | IDOR, Stored XSS and CSRF with significant impact; <br/>Internal SSRF and Lateral Authentication Bypass. |
| Medium   | Limited access to other user's private data                             | IDOR, Reflective XSS and CSRF with impact.                                                               |
| Low      | Configuration issues and other <br/>vulnerabilities with limited impact | SSL misconfigurations; <br/>XSS and CSRF with limited impact.                                            |

We award vulnerability reports at our discretion. In order to be eligible for a
bounty, your submission must be accepted as in-scope and valid.

The guidelines we use to determine the validity of reports are outlined below.

### Reproducibility

Our engineers must be able to reproduce the vulnerability you have reported.
Reports that include clearly written explanations and a working proof of concept
are more likely to be awarded.

### Severity and Priority

Generally, more impactful bugs will receive higher awards. Review the chart
above for examples of award levels for similar vulnerabilities.

### Award Factors

The amount awarded may vary depending upon the severity of the vulnerability
reported and quality of the report. If we receive multiple reports of the same
vulnerability, the first clear, reproducible report will be awarded.

We may decide to award higher for clever or more impactful vulnerabilities,
decide to award lower for vulnerabilities that require unusual user interaction,
decide that a single report constitutes multiple bugs or that multiple reports
are so closely related that they only warrant a single award.

## Disclosure

**Coordinated Disclosure:** Researchers may only share vulnerability details
with third parties after the vulnerability has been fixed and the Program has
provided permission to disclose OR 90 days after submission, whichever comes
first.

or

**Discretionary Disclosure:** Researchers may only share vulnerability details
with third parties after requesting and receiving explicit permission from the
Program.

## Guidelines

To encourage vulnerability research and to avoid any confusion between
legitimate research and malicious attack, we ask that you attempt, in good
faith, to:

- **Play by the rules.** Adhere to this policy and any other relevant
  agreements, e.g., Terms of Service;
- Report any vulnerability you’ve discovered promptly;
- Avoid violating the privacy of others, disrupting our systems, destroying
  data, and/or harming user experience;
- Use only the Official Channels to discuss vulnerability information with us;
- Handle the confidentiality of details of any discovered vulnerabilities
  according to our Disclosure Policy;
- Perform testing only on in-scope systems, and respect systems and activities
  which are out-of-scope;
- If a vulnerability provides unintended access to user data, such as Personally
  Identifiable Information (PII), Personal Healthcare Information (PHI), credit
  card data, or proprietary information: Cease testing and submit a report
  immediately;
- Only interact with accounts you own unless given explicit permission by the
  account holder;
- Do not engage in extortion.
- Be clear and succinct—a short proof-of-concept link is invaluable;
- Never attempt non-technical attacks—such as social engineering, phishing, or
  physical attacks—against our employees, users, or infrastructure; and
- Do not view, alter, save, store, transfer, or otherwise access our data or the
  data of our users without explicit permission.

We may modify the terms or terminate this program at any time.

## In-Scope

Any design or implementation issue that substantially affects the
confidentiality or integrity of user data is likely to be considered in-scope.
Common examples include:

- Cross-site scripting.
- Cross-site request forgery.
- Mixed-content scripts.
- Authentication or authorization flaws.
- Server-side code execution bugs.
- Circumvention of our permissions model.
- SQL injection.
- XML external entity attacks.

While this list is reflective of the research we prioritize, it should not be
considered exhaustive. Any report that concerns the possible compromise of
sensitive user data or our systems is of interest. By extension, this includes
the reporting of serious security weaknesses in any dependency—such as open
source libraries, software, or third-party components—actively used in the
development of our properties and/or products shared below.

## Out-of-Scope

The following issues are explicitly outside the scope of this program:

- Policies on presence/absence of SPF/DMARC records.
- Password, email and account policies, such as email id verification, reset
  link expiration, and password complexity.
- Logout cross-site request forgery.
- Attacks requiring physical access to a user's device.
- XSS on any site other than those listed as 'in-scope'.
- Attacks that require an exploitation tool to overlay on top of our app (e.g.,
  tapjacking).
- Vulnerabilities that require a potential victim to install non-standard
  software or otherwise take active steps to make themselves susceptible.
- Vulnerabilities affecting users of outdated browsers or platforms.
- Social engineering of our employees or contractors.
- Any physical attempts against our property or data centers.
- Presence of autocomplete attribute on web forms.
- Missing cookie flags on non-sensitive cookies.
- Any access to data where the targeted user needs to be operating a rooted
  mobile device.

The following issues are outside the scope of our program, unless they are
accompanied by evidence of exploitability:

- Use of a known-vulnerable library.
- Missing best practices.
- Insecure SSL/TLS ciphers.
- Missing security headers, which do not directly lead to a vulnerability.
- Lack of CSRF tokens, except when there is evidence of a sensitive user-action
  not protected by a token.
- Host header injections.
- Reports from automated tools or scans that haven't been manually validated.
- Presence of banner or version information, unless a vulnerable version.

## Known Issues

Any issues already known to us will be published as a separate Known Issues
list. These vulnerabilities are also considered out-of-scope, though new reports
of a known issue may be accepted if the instances described were not previously
observed.

## Safe Harbor

When conducting vulnerability research according to this policy, we consider the
research conducted under this policy to be:

- Authorized in view of any applicable anti-hacking laws, and we will not
  initiate or support legal action against you for accidental, good faith
  violations of this policy;
- Authorized in view of relevant anti-circumvention laws, and we will not bring
  a claim against you for circumvention of technology controls;
- Exempt from restrictions in our Acceptable Usage Policy that would interfere
  with conducting security research, and we waive those restrictions on a limited
  basis; and
- Lawful, helpful to the overall security of the Internet, and conducted in good
  faith.

You are expected, as always, to comply with all applicable laws. If legal action
is initiated by a third party against you, and you have complied with this
policy, we will take steps to make it known that your actions were conducted in
compliance with this policy.

If at any time you have concerns or are uncertain whether your security research
is consistent with this policy, please submit a report before going any further.

## The Fine Print

This is not a competition, but rather an experimental and discretionary program.

You are solely responsible for any applicable taxes, transaction fees, or other
withholdings that arise from or relate to your participation in this program.
