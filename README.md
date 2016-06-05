# gaelcód
C as Gaeilge

Mar shampla:

```
#iniaigh <caighdeán_ionchur_aschur.h>

príomh()
{
        cuir_i_gcló("Dia duit an domhain\n");
        cuir_air_ais 0;
}
```

```
#iniaigh <caighdeán_ionchur_aschur.h>

príomh()
{
        slánuimhir n, c;

        cuir_i_gcló("Iontráil uimhir\n");
        scan("%d", &n);

        má (n == 2) {
                cuir_i_gcló("Is uimhir phríomha í\n");
        } eile {
                do (c = 2; c < n; c++) {
                        má (n % c == 0) {
                                bris;
                        }
                }
                má (c != n) {
                        cuir_i_gcló("Níl uimhir phríomha í\n");
                } eile {
                        cuir_i_gcló("Is uimhir phríomha í\n");
                }
        }
        cuir_ar_ais 0;
}
```

## Úsáid:

```bash
$ ./gaelcc -i samplaí/dia_duit_an_domhain.c -o triail; ./triail
```
