# Timestamps

[OpenTimestamps](https://opentimestamps.org) proofs for the assets of release `v1`.
Each proof commits to the SHA-256 of the file below.

| file | SHA-256 |
|---|---|
| `goldbach-1plus1.75-theorem-v1.pdf` | `6791bd40b5c90da774e384edbd1d40a47216465770022b11bda6052a5bddc1a1` |
| `paper-iii-source-v1.tar.gz` | `6e4eca2ff7fa83ed65cf21ba4f9d20ba8bedaabf7425f3db7bf99b56986e3082` |
| `paper-iii-public-certificates-v1.tar.gz` | `bd45baa10b3084df9a8fc626196dc31e20317db49a6929f1d347d316280d9162` |

To verify, download the release asset into this directory and run

    pip install opentimestamps-client
    ots verify timestamps/<file>.ots
