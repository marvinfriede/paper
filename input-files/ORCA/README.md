ORCA Input Files
================

Example input files for ORCA calculations with the cam-B3LYP and &omega;B97M-D4 functionals.

Note that some options (e.g. `maxcore`) are omitted for clarity.

Problematic cases were converged with (some of) the following additional options:

```
!KDIIS SOSCF NoTrah SlowConv

%scf
  DIISMaxEq 15
  directresetfreq n   # n=1,2,3 
  soscfmaxit 12
end
``` 