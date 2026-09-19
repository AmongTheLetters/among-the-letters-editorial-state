# Among The Letters - Public Editorial State

This repository contains only the publication-state data that an editorial agent needs for duplicate prevention and publication tracking. It is intentionally safe for public read access.

## Files

- `publication_history.csv` - authoritative record of items that actually appeared in published Among The Letters editions.
- `featured_history.csv` - append-only record of items that appeared as Featured content.
- `review_flags.csv` - public-safe editorial ambiguity flags only. Do not put private notes, subscriber information, credentials, or personal data here.
- `current/recent_14_days.csv` - derived convenience view of the most recent 14 days. It is not authoritative.

## Agent rules

1. Read `publication_history.csv` before selecting content.
2. Check exact primary-source URL first, then normalized title + organization.
3. Previously published material is excluded by default unless an explicit editorial reuse exception applies.
4. Do not add researched candidates, rejected items, drafts, backups, or items removed during human review.
5. Update state only after the human confirms the final edition was published.
6. Preserve historical rows. Never delete an old row because an external item later closes or changes.
7. `current/recent_14_days.csv` must be regenerated from `publication_history.csv`; it must never replace the full history as the duplicate source.
8. Do not store secrets, API keys, subscriber data, email addresses, private business notes, unpublished manuscripts, or credentials in this public repository.

## Current bootstrap state

The repository currently contains confirmed publication records for September 18 and September 19, 2026. The September 19 Afternoon Discoveries rows were moved into authoritative history only after publication was confirmed.

The September 18 bootstrap was reconstructed from the published materials available in the project. If older published editions exist and are not yet represented, backfill them before treating this as a complete lifetime archive.
