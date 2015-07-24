# haploSNP

This file contains an executable jar file that will build haploSNPs from the phased eigenstrat data that is used as input. 
Usage is:

```
java -jar HaploSNP.jar parfile
```


a sample parfile looks like:
```
phsnpfile=../phase/chr22.phsnp
phgenofile=../phase/chr22.phgeno.gz
phindfile=../phase/chr22.phind
minmaf=0.001
outpre=chr22
maxlength=50000
```

Parameters `phsnpfile`, `phgenofile`, `phindfile`, and `outpre` are required. Parameters `minmaf` and `maxlength` are recommended. Note that very low MAFs and very high lengths will result in a large number of haploSNPs.
