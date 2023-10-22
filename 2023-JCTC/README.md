# Supporting Information

SI for the paper:

**Do optimally-tuned range-separated hybrid functionals require a re-parameterization of the dispersion correction? It depends.**
<br>
*M. Friede, S. Ehlert, S. Grimme, J.-M. Mewes*
<br>
J. Chem. Theory Comput. 2023.


## Contents

This repository contains example input files for calculations with the range-separated hybrid functionals investigated in the paper.

Additionally, the potential energy surfaces for all six functionals are shown for the whole DFT-D4 fit set consisting of S22x5, S66x8, and NCIBLIND10.


## Overview: Range-separated Hybrid Functionals

A non-exhaustive list of range-separated functionals available by keywords in ORCA, TURBOMOLE and Q-CHEM.
<br>
<br>

| Functional        |   ORCA   | Turbomole |  Q-Chem  | default &omega; |
| ----------------- | :------: | :-------: | :------: | :-------------: |
| CAM-B3LYP         | &check;  |  &check;  | &check;  |      0.33       |
| rCAM-B3LYP        | &#10007; | &#10007;  | &check;  |                 |
| CAMQTP-00         | &#10007; |  &check;  | &check;  |                 |
| CAMQTP-01         | &#10007; |  &check;  | &check;  |      0.31       |
| CAMQTP-02         | &#10007; |  &check;  | &#10007; |                 |
| LC-BLYP           | &check;  | &#10007;  | &#10007; |      0.33       |
| LC-(&omega;)PBE   | &check;  |     ?     | &#10007; |      0.47       |
| LC-(&omega;)PBE08 | &#10007; |     ?     | &check;  |      0.45       |
| LRC-(&omega;)PBE  | &#10007; |     ?     | &check;  |      0.30       |
| LRC-(&omega;)PBEh | &#10007; |  &check;  | &check;  |      0.20       |
| LRC-BOP           | &#10007; | &#10007;  | &check;  |      0.47       |
| &omega;B97        | &check;  |  &check;  | &check;  |      0.40       |
| &omega;B97X       | &check;  |  &check;  | &check;  |      0.30       |
| &omega;B97X-V     | &check;  |  &check;  | &check;  |      0.30       |
| &omega;B97X-D     | &#10007; |     ?     | &check;  |      0.20       |
| &omega;B97X-D3(0) | &check;  | &#10007;  | &check;  |      0.25       |
| &omega;B97X-D3BJ  | &check;  | &#10007;  | &#10007; |      0.30       |
| &omega;B97M-D3BJ  | &check;  | &#10007;  | &#10007; |      0.30       |
| &omega;B97M-D4    | &check;  | &#10007;  | &#10007; |      0.30       |
| &omega;B97M-V     | &#10007; |  &check;  | &check;  |      0.30       |

<br>
Additional notes:

- Default &omega; values from ORCA 5.0.1 Manual and Q-Chem 5.4 Manual (no values given in Turbomole 7.5.1 Manual)
- Q-CHEM: LC-&omega;PBE08 (&omega;=0.45) and LRC-&omega;PBE (&omega;=0.30) only differ in &omega;
- LC-PBE has different names and variants with different &omega;'s
