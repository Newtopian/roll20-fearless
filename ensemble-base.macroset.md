## D10
```
[[ 1D10!cf<1cs>10 ]]
```
## allmod
```
[[ #modEGO + #modMENTAL + #modNLETAUX + #modLETAUX + #modCHI ]]
```
## modCHI
```
[[ floor( ( (abs(9 - @{selected|CHI}) + (9 - @{selected|CHI})) / 2) / -3) ]]
```
## modEGO
```
[[ floor( ( (abs(7 - @{selected|EGO}) + (7 - @{selected|EGO})) / 2) / -4) ]]
```
## modLETAUX
```
[[ floor( ( (abs(7 - @{selected|LETAUX}) + (7 - @{selected|LETAUX})) / 2) / -2) ]]
```
## modMENTAL
```
[[ floor( ( (abs(7 - @{selected|MENTAL}) + (7 - @{selected|MENTAL})) / 2) / -2) ]]
```
## modNLETAUX
```
[[ floor( ( (abs(7 - @{selected|NLETAUX}) + (7 - @{selected|NLETAUX})) / 2) / -4) ]]
```

## Initiative
L'initiative verra le calcul automatiquement ajouté au tracker d'initiative si il est activé.
Le jet d'initiative comme lest autres doit se faire une fois le token sélectionné.
```
Initiative([[#D10 + @{selected|REF} + @{selected|INT} + #allmod &{tracker}]]) 
```

## Image
```
[Image](?{Image URL|})
```
