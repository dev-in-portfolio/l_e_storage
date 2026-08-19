# Lulu & Ellie Library Import Status

Source: ChatGPT Library folder `/Lulu and Ellie`

Date prepared: 2026-08-19

## First-pass target

- 142 Library entries inventoried.
- 15 PDFs exceed GitHub's normal 100 MiB single-file limit and are deferred for later handling.
- 127 entries are below the normal GitHub limit.
- 1 of those 127 is a confirmed byte-for-byte duplicate.
- Therefore the clean first-pass target is **126 unique under-limit files**.
- All four MP3 song variations are intentionally retained as separate files.

## Confirmed duplicate — skip one copy

Keep:
`Lulu_and_Ellie_Go_To_Camp_Book_8_The_Canoe_That_Sang_to_the_Moon_FINAL.pdf`

Skip duplicate:
`Lulu_and_Ellie_Go_To_Camp_Book_8_The_Canoe_That_Sang_to_the_Moon_FINAL(1).pdf`

Both copies have SHA-256:
`38ad961425664ba203ee3ca9a5f730dad9e93efee9f6200ab5e45d18432ba1e1`

## Preserve all four song variations

- `Lulu and Ellie Paws Up.mp3`
- `Lulu and Ellie Paws Up (1).mp3`
- `Lulu Ellie Portal.mp3`
- `Lulu Ellie Portal (1).mp3`

These are intentional variations and must not be deduplicated by filename similarity.

## Deferred — oversized PDFs

The following 15 files exceed 100 MiB and are deferred rather than blocking the rest of the import:

1. `Lulu_&_Ellie_In_Space_Book9.pdf` — 153,758,294 bytes
2. `Lulu_&_Ellie_in_Space_Book13.pdf` — 150,308,824 bytes
3. `MysteryTails1_REPAIRED.pdf` — 149,413,924 bytes
4. `Lulu_Ellie_Creature_Rescue_Club_Book12_The_Moonbrella_Moth_Final.pdf` — 146,872,301 bytes
5. `Lulu_&_Ellie_In_Space_Book2.pdf` — 139,907,656 bytes
6. `Lulu_Ellie_Go_To_Camp_Book_11_Final.pdf` — 123,942,334 bytes
7. `Cook2.pdf` — 118,731,958 bytes
8. `Lulu_Ellie_Creature_Rescue_Club_Book17_The_Cloudlet_Fawn_in_the_Clover_Clock_FINAL.pdf` — 118,445,646 bytes
9. `Lulu_Ellie_Go_To_Camp_Book_10_The_Lantern_That_Pointed_Sideways_FINAL.pdf` — 116,979,589 bytes
10. `Lulu_Ellie_Mystery_Tails_Book16_The_Case_of_the_Lantern_That_Winked_FINAL.pdf` — 116,214,908 bytes
11. `Lulu_Ellie_Creature_Rescue_Club_Book_20_The_Moon_Moss_Mender.pdf` — 116,031,006 bytes
12. `Lulu_Ellie_Mystery_Tails_Book19_Final.pdf` — 113,515,803 bytes
13. `Lulu_and_Ellie_Go_To_Camp_5.pdf` — 112,974,632 bytes
14. `Time_Tails_Book_9_The_Acorn_That_Ticked_Tomorrow_FINAL.pdf` — 112,122,758 bytes
15. `Academy5.pdf` — 109,091,993 bytes

## Repository handling

The `l_e_storage` branch is configured with Git LFS patterns for `*.pdf` and `*.mp3`. The oversized list above remains explicitly deferred so it does not block the under-limit archive pass.
