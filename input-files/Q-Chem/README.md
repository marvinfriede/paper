Q-Chem Input Files
==================

Example input files for Q-Chem calculations with a variety of functionals.

Note that some options (e.g. `threads` or `scf_max_cycles`) are omitted for clarity.

For the large systems of the L7 benchmark, the SCF calculations converged very slowly with `scf_convergence 8` as used for NCIBLIND10, S22x5 abd S66x8. The even larger complexes of the S30L benchmark set were even more problematic. The additional lack of accelaration methods for the exchange part in Q-Chem (like ORCA's `RIJCOSX`) forced us to adapt looser convergence thresholds. These thresholds are still accurate (10<sup>-6</sup> Hartree = 0.6 mkcal/mol), especially as we are only interested in single point energies.

- L7: `scf_convergence 7`
- S30L: `scf_convergence 6`

In fact, Q-Chem only recommends `scf_convergence 5` for single point energies. The cutoff for the neglect of two-electron integrals `thresh` is left at 10<sup>-11</sup>.

Other algorithms (e.g. Geometric Direct Minimization) did not provide improvements concerning SCF convergence.
