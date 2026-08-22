# **Privacy Matters** Now More Than Ever

Welcome to the official GitHub repository for the **Institute for Signature Reduction (ISR)** single-page website.

Yes, it's just one page. Yes, it's simple. That's the point.

---

## About ISR

The **Institute for Signature Reduction (ISR)** is an independent 501(c)(3) nonprofit charitable organization advancing education, research, and training in:

- Digital force protection
- Cyber privacy
- Signature reduction

ISR publishes doctrine, stewards the corpus, and licenses the framework for applied instruction. The Institute does not deliver training directly.

---

## Purpose of this Repository

This repository hosts the **ISR static site** and the archive PDFs of the ISR corpus:

- Single-page layout
- No WordPress, no plugins, no build step
- Served via GitHub Pages

A digital calling card, and the source of record for the publications.

---

## Architecture

- Static HTML, CSS, and a small amount of inline JavaScript
- Single file — no build step, no package manager, no dependency tree
- No server-side code
- No databases or persistent storage
- No authentication mechanisms
- No cookies, local storage, or session storage
- No client-side tracking, analytics, or telemetry

The JavaScript is inline and does four things: the mobile navigation menu, the back-to-top button, runtime assembly of the contact address, and the contact form submission.

---

## Third-Party Requests

**One.** The contact form posts to a third party service on submit. Nothing else on the page contacts any host other than the one serving it.

### About the form

The third party service receives everything submitted — name, email, message — and additionally logs IP address, browser type, access time, and referrer. Submissions are retained in an account, not merely relayed. The site states this at the point of collection so a visitor can make an informed choice, and offers direct email as the alternative.

This is a deliberate trade: a form lowers the barrier for the general research and licensing correspondence we want to receive. It is not appropriate for anything sensitive, and we say as much.

---

## Publications

The archive PDFs in `/publications/` are the source of record; journal mirrors may change.

PDFs may carry embedded metadata although we strip most of it prior to publication: author name, creating application, revision timestamps, and sometimes the full local file path of the machine that produced them. **Check every PDF before committing it.**

```
exiftool publications/isr-doc-00X.pdf     # inspect
exiftool -all= publications/isr-doc-00X.pdf   # strip
```

The same applies to `images/terrain.jpg` and any other image added to the repository.

---

## What This Does Not Cover

Stating the limits honestly is part of the discipline this site is about.

- **Host logs.** GitHub Pages records visitor IP addresses, user-agents, and requested paths in its own infrastructure. This is outside the site's control.
- **Repository metadata.** This repository is public, and so is its commit history. Every commit carries an author name, an author email, and a timestamp, and commit timing across a history reveals a working-pattern signature. Verify what identity is attached to commits before pushing; GitHub's no-reply address closes this going forward.
- **Archives.** Prior versions of this site, including content since removed, are likely captured by the Internet Archive and similar services. Removing content going forward does not retract what was published.
- **Transport.** Email is not a secure channel, and neither is a web form.

---

## Force Protection Considerations

- This site functions strictly as a publication and contact relay
- No operational, personnel, or sensitive business data is hosted
- Repository contents should be treated as publicly accessible at all times
- Changes should be reviewed with OPSEC and digital footprint considerations in mind

### Pre-commit checklist

1. Does the change add any request to a host other than this one? If yes, stop.
2. Does it introduce a build step, package manager, or external dependency?
3. Does it place the contact address in plain text anywhere in the markup?
4. Have any added PDFs or images been checked for embedded metadata?
5. Does it add a claim about the organization, affiliation, personnel, or exempt status that cannot be substantiated?
6. Does it add cookies, storage, or any form of visitor state?
7. Does any governance language commit to a date or a process with an endpoint? Present-tense structure only.
8. Is the identity attached to this commit the one intended to be public?

---

## About the Content

Select editorial, analytical, and design workflows for this site are supported by AI-enabled tools under **human direction and review**.

---

## License

**All rights reserved.**

Copyright © Institute for Signature Reduction. The source code, markup, styling, written content, design, publications, and all other materials in this repository are proprietary. No license is granted, expressly or by implication.

You may not copy, modify, distribute, publish, sublicense, or create derivative works from any part of this repository without prior written permission from ISR. Viewing the source in a browser, as any visitor may, does not constitute a grant of any right to reuse it.

This repository is public for transparency and delivery, not for reuse. The absence of a permissive license file is deliberate; under copyright law, no license means no permission.

Publications in `/publications/` are made freely available to read and cite. Citation as `ISR-DOC-[number], Institute for Signature Reduction` is welcome and encouraged. Redistribution, republication, or derivative use of the documents themselves requires permission.

### One limit worth knowing

Because this repository is hosted publicly on GitHub, GitHub's Terms of Service grant other GitHub users the ability to view and fork it *within the platform*, regardless of the terms above. "All rights reserved" governs use outside that mechanism; it does not disable the fork button.

---

## Repository Use, Attribution, and Branding

- This repository is the sole authoritative source for the **official ISR website**. All official content, updates, and maintenance are performed exclusively by the ISR team or authorized representatives. This repository and the associated live site are the only sources through which official ISR web content and contact information are published.

- No permission is granted to reuse this codebase or its content. Should any copy or derivative nonetheless be published, it does not carry permission to represent, brand, or imply affiliation with ISR, nor to present itself as an official ISR site. Any such copy must clearly identify itself as unofficial and remove ISR branding and identifying marks in full.

- ISR names, logos, written content, publications, and other identifying materials are proprietary and are not licensed under any terms. No third party is authorized to claim to act on behalf of, speak for, or represent ISR through a copied or derivative version of this site.

---

🇺🇸 **Privacy Matters.**
