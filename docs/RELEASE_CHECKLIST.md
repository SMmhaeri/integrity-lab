# Integrity Lab Release Checklist

Use this checklist before making a packaged build publicly accessible.

## 1. Confidentiality and data

- Confirm the package contains no proprietary industry ILI datasets unless explicit redistribution permission exists.
- Confirm no private supervisor, collaborator, or industry files are bundled.
- Confirm no API keys, tokens, passwords, `.env` files, private keys, local credentials, or machine-specific secrets are present.
- Confirm demonstration data are synthetic, public, or explicitly redistributable.

## 2. Package integrity

- Keep the complete packaged directory structure intact.
- Verify `IntegrityLab.exe` launches from a freshly extracted copy of the ZIP.
- Verify the bundled `runtime/`, `frontend/`, `backend/`, and launcher components are present if required by the build.
- Verify `LICENSES/`, `NOTICE.txt`, `RELEASE_MANIFEST.json`, and user-facing instructions are included.
- Run the packaged smoke tests and update `TEST_STATUS.txt` if that file is part of the release process.

## 3. Public-facing documentation

- Update the repository README if capabilities or system requirements changed.
- Add representative screenshots or a short demonstration asset when available.
- Document the release version and date.
- Record any known limitations.

## 4. Current research release

```text
Tag:          v1.0.0
Title:        Integrity Lab v1.0.0 — Research Release
Asset:        IntegrityLab.zip
SHA-256:      340db243570d7e04b32b964789483986afd19e28b79d2a12cf954ec3574ce383
```

The complete packaged ZIP is distributed as a **GitHub Release asset** rather than committing the bundled runtime to ordinary Git history.

## 5. Licensing

Do not assign an open-source license until ownership, third-party licensing, coauthor/supervisor expectations, and industry/IP restrictions have been checked. Preserve all third-party notices included in the packaged application.
