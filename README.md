# Vernota Proof Archive

This repository is an independent, append-only public record of cryptographic 
fingerprints (SHA-256 hashes) of statements recorded in the Vernota app.

## What is stored here

Each file in `records/YYYY/YYYY-MM-DD.csv` contains one row per statement 
recorded on that date:

- `date` — the recording date (YYYY-MM-DD)
- `content_hash` — SHA-256 fingerprint of the statement

No statement text, no user data, no personal information is stored here.
The hash alone is meaningless without the original content.

## Why this exists

Vernota allows users to cryptographically timestamp statements and verify them 
later. This public archive provides an independent timestamp — owned by GitHub 
(Microsoft), outside Vernota's control — proving that a given hash existed on 
a specific date.

## How to verify

1. Find the proof page: vernota.app/proof/[token]
2. Note the SHA-256 fingerprint and recording date
3. Open the CSV file for that date in this repository
4. Confirm the fingerprint appears in that file
5. GitHub's commit timestamp confirms when it was recorded

For full verification instructions: vernota.app/verify
