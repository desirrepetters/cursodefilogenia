---
title: "MrBayes - Modelos de Substituição"
linkTitle: "MrBayes - Modelos de Substituição"
weight: 4
description: >
  Codificação utilizada para informar o modelo evolutivo a ser utilizado pelo MrBayes em uma análise filogenética
---


## MrBayes - Modelos de Substituição


### GTR

##### GTR

```
lset nst=6
```

##### GTR + G

```
lset nst=6 rates=gamma
```

##### GTR + I

```
lset nst=6 rates=propinv
```

##### GTR + I + G

```
lset nst=6 rates=invgamma
```

```
 [GTR]

lset nst=6 rates=propinv [GTR + I]

lset nst=6 rates=gamma [GTR + G]

lset nst=6 rates=invgamma [GTR + I + G]

```


### SYM

```
lset nst=6 
prset statefreqpr=fixed(equal)

lset nst=6 rates=propinv [GTR + I]

lset nst=6 rates=gamma [GTR + G]

lset nst=6 rates=invgamma [GTR + I + G]

```