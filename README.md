# Behave C-3PO — Public Sealed-Predictions Record

This repo is the **public verification record** for sealed predictions made by the
Behave Population Engine. It contains exactly one thing of substance: `SEALS.md`,
the sealed-predictions manifest.

## What this is for

Every time a prediction is sealed **before its truth is known**, its SHA-256 hash is
committed to `SEALS.md` — with the event name, the commit timestamp, and the date
truth is expected. When truth resolves, the same row is updated with its grade.

A stranger can therefore verify two things:

1. **The denominator** — how many predictions were actually sealed (no retroactive
   editing of the record).
2. **Full revelation** — every sealed prediction gets revealed and graded, hit or
   miss. A miss that is honestly shown is worth more than a record that hides.

## How to verify

At seal time, the hash prefix is published. Compare it against the row in
`SEALS.md` here. The manifest is only ever appended or graded — never rewritten.

## What is NOT here

The engine itself, its populations, methodology, and clients' data are proprietary
and remain private. This repo exists solely so the seal record is independently
checkable by anyone.

---

*Maintained by the Behave Population Engine — see the private engine repo's
`experiments/seal_manifest.py` for how this file is generated.*
