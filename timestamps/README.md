# Timestamps

[OpenTimestamps](https://opentimestamps.org) proofs for the assets of release `v1`.
Each proof commits to the SHA-256 of the file below.

| file | SHA-256 |
|---|---|
| `goldbach-1plus1.75-theorem-v1.pdf` | `6791bd40b5c90da774e384edbd1d40a47216465770022b11bda6052a5bddc1a1` |
| `paper-iii-source-v1.tar.gz` | `6e4eca2ff7fa83ed65cf21ba4f9d20ba8bedaabf7425f3db7bf99b56986e3082` |
| `paper-iii-public-certificates-v1.tar.gz` | `bd45baa10b3084df9a8fc626196dc31e20317db49a6929f1d347d316280d9162` |

Proofs for the new assets of release `v2` (anchored in Bitcoin block 975641, 2026-11-13 07:25:27 UTC; the certificate archive is unchanged and its proof is listed above):

| file | SHA-256 |
|---|---|
| `goldbach-1plus1.75-theorem-v2.pdf` | `6228b5dc7f594a5ec7f44577133c6b12096f7c110a2cfeef8764489b03d98b4e` |
| `paper-iii-source-v2.tar.gz` | `c03160062560acada7f1069efe4a33e7a8c0031339c81472ff859f977b313453` |

To verify, download the release asset into this directory and run

    pip install opentimestamps-client
    ots verify timestamps/<file>.ots
