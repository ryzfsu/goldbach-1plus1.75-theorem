# Erratum to "Theorem (1 + 1.75) on the Goldbach conjecture" (version 1)

Ruiyi Zhang · November 13, 2026 · concept DOI 10.5281/zenodo.24184562

In the proof of Lemma 6.10 (page 45 of version 1), the display that applies
Lemma 6.9 reads

    |sum_{r,s} F(r,s) D_cell(rs,N)| <= sum_r max_{(b,r)=1} sum_s max_{a} |D_cell(rs,a)| << N L^{-T_save}.

The modulus sums should carry the ranges and conditions of Lemma 6.9, (6.48):

    ... <= sum_{r ~ Q_1} max_{(b,r)=1} sum_{s ~ Q_2, mu(rs)^2 = 1, (rs,N) = 1} max_{a} |D_cell(rs,a)| << N L^{-T_save}.

As printed, the right-hand side is a larger sum than Lemma 6.9 covers. The
coefficient F(r,s) is supported on squarefree rs with (rs,2N) = 1, and |F| <= 1,
so the corrected sum majorizes the left-hand side and Lemma 6.9 applies with
x = N, as the surrounding text already states ("Both classes are reduced since
(rs,N) = 1"). No estimate, constant or numerical value changes, and Theorem 1
is unaffected.

Version 2 contains the corrected display. It also makes three wording and
notation corrections, none of which changes an estimate or a constant:

- proof of Lemma 6.8: the bad-tuple cost is written with the parent length H
  instead of T_int, as in the lemma and in the supplementary proof;
- Section 5 (page 27): the sentence on the fixed deduction g_tau is clarified;
- Section 9: the optional sharper comparison is described as historical and
  non-certified; the main count uses c_K2,G0 throughout.

The date line is updated. Because the Section 5 sentence adds two lines, page
numbers from page 27 onward may differ by one between the versions; version 2
has 106 pages (version 1: 105).
