# Lulu & Ellie Library Import Status

Date updated: 2026-08-30

## Original Adventure core set

- **20 of 20 full Original Adventure books are present** in `library-import/`.
- Books 1, 11, and 16 were preserved from the existing archive.
- Books 2–10, 12–15, and 17–20 were added from the verified Library source set.
- Every full-book PDF is tracked through Git LFS and has a recorded source byte count and SHA-256 in `CORE_PDF_MANIFEST.md`.
- Oversized Books 14, 19, and 20 were transferred in verified temporary chunks, reconstructed byte-for-byte, verified against the full source SHA-256, and then the temporary chunks were removed.
- No `.transfer/` manifests or reconstruction chunks are part of the completed canonical set.

## Transfer workflow

The repository workflow supports both direct verified Drive relays and verified chunk assembly for files above the normal single-file transport limit. Each import checks exact byte count and SHA-256 before committing the resulting LFS object.

## Broader Library inventory

The earlier 2026-08-19 inventory covered the larger Lulu & Ellie Library beyond the Original Adventure core set. Its counts for other series/media remain a separate archive workstream and should not be read as the status of these 20 Original Adventure books.

The Original Adventure core set is complete.
