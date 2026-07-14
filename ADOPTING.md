# Adopting Core License

This checklist turns the template into a project-specific licensing package.

## Required Decisions

Before publishing, decide and document:

- Project name.
- Legal name of the copyright holder or licensing entity.
- License contact email.
- Whether AGPLv3 is "version 3 only" or "version 3 or later". This template uses `AGPL-3.0-only`.
- Who can sign evaluation order forms, commercial order forms, and philanthropy waiver certificates.
- Whether affiliates, contractors, hosted services, plugins, embedded products, customers, or distributors are covered by signed proprietary-use grants.

## Required Files

A project adopting this package should include:

- `LICENSE.txt`: verbatim AGPLv3 text.
- `README.md`: a short licensing section that points to the files below.
- `LICENSE-EVALUATION.txt`: public evaluation license terms.
- `EVALUATION-ORDER-FORM.template.md`: signed evaluation form.
- `LICENSE-COMMERCIAL.txt`: public commercial license terms.
- `COMMERCIAL-ORDER-FORM.template.md`: signed commercial license form.
- `LICENSE-PHILANTHROPY-WAIVER.txt`: public philanthropy waiver terms.
- `PHILANTHROPY-WAIVER-CERTIFICATE.template.md`: signed waiver certificate form.
- `CONTRIBUTING.md`: inbound contribution terms.
- `NOTICE`: project copyright and licensing notice, based on `NOTICE.template`.

## Source Headers

Use the AGPL SPDX identifier for source files unless a file is intentionally under different terms:

```text
SPDX-License-Identifier: AGPL-3.0-only
```

For files where a copyright notice is normal, use:

```text
Copyright (C) [year] [copyright holder]
SPDX-License-Identifier: AGPL-3.0-only
```

## Contributor Rights

The commercial license and philanthropy waiver can only cover code the licensor has the right to license that way. If outside contributors retain copyright and only contribute under AGPLv3, the project may not be able to grant proprietary-use rights to their contributions.

Use `CONTRIBUTING.md`, a CLA, copyright assignment, or another reviewed inbound licensing process before accepting contributions that should be covered by the commercial and waiver paths.

## Release Checklist

Before a release:

1. Confirm every distributed source file has the correct license identifier or notice.
2. Confirm generated files, vendored dependencies, examples, assets, and docs have compatible licensing.
3. Confirm evaluation and proprietary-use grants are issued only through signed order forms or waiver certificates.
4. Keep signed documents and donation receipts in a private records system.
5. Publish no public donation amounts or commercial terms unless the project intentionally chooses to do so later.

## README Snippet

Projects can adapt this text:

```markdown
## License

This project is licensed under AGPLv3 by default. See `LICENSE.txt`.

Evaluation licenses, commercial licenses, and philanthropy waivers are available separately. See `LICENSE-EVALUATION.txt`, `LICENSE-COMMERCIAL.txt`, and `LICENSE-PHILANTHROPY-WAIVER.txt`. Those alternatives are effective only when signed by the project licensor.
```
