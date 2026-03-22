# testing2-for-erors

## Galutinis release
Po pradinio relese išleidimo buvo padarytas programos optimizavimas 3 skirtingomis strategijomis su fiksuotu konteneriu - std::vector. 

| Failo dydis      | 1 strategija (s) - for ciklas | 2 strategija (s) - erase | 3 strategija (s) - std::partition |
|------------------|-------------------------------|--------------------------|-----------------------------------|
| 1 000            | 0.0030354                     | 0.0371157                | 0.0025987                         |
| 10 000           | 0.0240486                     | 3.45011                  | 0.0255509                         |
| 100 000          | 0.28094                       | 385.784                  | 0.276189                          |
| 1 000 000        | 2.72145                       |               | 3.0776                    |
| 10 000 000       | 31.6804                       |               | 33.412                    |
