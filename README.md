# Theorem (1 + 1.75) on the Goldbach conjecture

Ruiyi Zhang

DOI: [10.5281/zenodo.24184562](https://doi.org/10.5281/zenodo.24184562)

Every sufficiently large even integer `N` has a representation

    N = p + r q,    p, q prime,    r = 1 or r prime,    r <= q^(3/4).

In the terminology of Li and Liu, this proves Proposition (1 + a) for `a = 1.75 = 7/4`
(Li-Liu prove `a = 1.9`; Paper II [Z2] proves `a = 1.8`).

A weighted sieve combines thirteen signed row estimates with a switched upper bound. The directed
comparison gives

    D_B          > 1.967088903489691335582703173494,
    c_{K2,G0} I(b) < 1.966859949178424046530804965344,

so the exact margin enclosure is `D_B - c_{K2,G0} I(b) > 0.000228954311267289051898208151`.
The proof uses the Siegel-Walfisz theorem, so the threshold for "sufficiently large" may be
ineffective.

[Z1] R. Zhang, *Shifted primes in arithmetic progressions to large moduli with linear sieve
remainder weights*, Zenodo, 2026. DOI: 10.5281/zenodo.23615525.

[Z2] R. Zhang, *Theorem (1 + 1.8) on the Goldbach conjecture*, Zenodo, 2026.
DOI: 10.5281/zenodo.23649264.

## Revision

Version 2 (November 13, 2026; release `v2`) makes one mathematical display correction and three
wording/notation corrections. None changes a constant, a hypothesis or Theorem 1. See `ERRATUM.md`.

- Proof of Lemma 6.10 (page 45): the modulus sums in the display applying Lemma 6.9 now carry
  `r ~ Q_1`, `s ~ Q_2`, `mu(rs)^2 = 1` and `(rs,N) = 1`, exactly as in (6.48).
- Proof of Lemma 6.8: the bad-tuple cost is written with the parent length `H` instead of `T_int`.
- Section 5: the sentence on the fixed deduction `g_tau` is clarified.
- Section 9: the optional sharper comparison is described as historical and non-certified.

Version 1 (November 12, 2026; release `v1`, 105 pages) remains available unchanged.

## Contents

- `main.pdf` (version 2, 106 pages)
- `source/` - LaTeX source: `main.tex`, `paperiii-notation.tex`, `references.tex` and `chapters/`
- `ERRATUM.md` - erratum to version 1
- `LICENSE.md`, `LICENSES/`
- `SHA256SUMS`

The release `v2` (current) carries the PDF, the LaTeX source package `paper-iii-source-v2.tar.gz`, and the
numerical-certificate supplement `paper-iii-public-certificates-v1.tar.gz` (scripts, exact inputs,
compact outputs and verification records) at the address printed in the paper's Data availability
statement (the certificate archive is unchanged and is also attached to release `v1`):

https://github.com/ryzfsu/goldbach-1plus1.75-theorem/releases/download/v1/paper-iii-public-certificates-v1.tar.gz

The SHA-256 of the supplement archive is
`bd45baa10b3084df9a8fc626196dc31e20317db49a6929f1d347d316280d9162`; the `SHA256SUMS` manifest inside
it has SHA-256 `81fc00441c3a3f0924995cd41263feddece827d9b40376dae531191c86f90ed3` (the hash printed in
the paper). Inside the unpacked archive, `python3 verify_bundle.py` checks the manifests, all 512 exact
rows, the recorded M5 regeneration, the derivative certificate and the 400-box enclosure.

## Build

    cd source
    pdflatex main.tex
    pdflatex main.tex
    pdflatex main.tex
    pdflatex main.tex

## Citation

Ruiyi Zhang, *Theorem (1 + 1.75) on the Goldbach conjecture*, preprint, Zenodo, 2026. https://doi.org/10.5281/zenodo.24184562

```bibtex
@misc{zhang2026goldbach175,
  author    = {Zhang, Ruiyi},
  title     = {Theorem (1 + 1.75) on the Goldbach conjecture},
  year      = {2026},
  publisher = {Zenodo},
  note      = {Preprint},
  doi       = {10.5281/zenodo.24184562},
  url       = {https://doi.org/10.5281/zenodo.24184562}
}
```

## License

Text, data and certificates: CC BY 4.0. Software: Apache License 2.0. See `LICENSE.md`.
