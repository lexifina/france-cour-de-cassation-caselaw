# Reproducing this repository

Input: the DILA archives of the base(s) CASS (decisions published in the Bulletin) and INCA (unpublished decisions) (the full dump `Freemium_*_global_20250713-140000.tar.gz` and every
increment after it, up to 2026-11-05), from https://echanges.dila.gouv.fr/OPENDATA/; france-law `main` for the overlay.

```
python tools/parse.py <archives> <parsed>
python tools/build.py cour-de-cassation <parsed> <empty folder> --today 2026-11-06 --updated 2026-11-05
```

Gives 530,372 decision commits and one documentation commit.
