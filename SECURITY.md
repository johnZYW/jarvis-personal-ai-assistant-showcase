# Security and privacy note

This public repository has been prepared for portfolio and competition review.

The following items are intentionally excluded:

- API keys and credential files
- Google service account JSON files
- local SQLite memory databases
- audio recordings and generated voice files
- user calendar/email/travel data
- production backend implementation
- latest iOS app source code
- logs, caches, and private working documents

Use environment variables for credentials. Never commit `.env`, `keys/`, `API_key/`, or service-account JSON files.

If a credential has ever been stored in a local working folder or zip archive, rotate/revoke it before public release.
