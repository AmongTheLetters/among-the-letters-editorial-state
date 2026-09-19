# Agent Read/Update Contract

Use this repository as persistent editorial state for Among The Letters.

- `publication_history.csv` is authoritative.
- Never infer that a draft was published.
- Only prepare state changes after explicit human confirmation of publication.
- For duplicate detection, compare canonical URL and normalized title + organization.
- Prefer new verified material. Reuse only under the publication's documented editorial exception rules.
- Keep this repository public-safe. Never add secrets, subscriber data, private contact details, unpublished submissions, or sensitive notes.
- A human always reviews, commits, and pushes all changes.
