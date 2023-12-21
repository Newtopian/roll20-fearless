## D10
```
[[ 1D10cf<1cs>10 ]]
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
[[ floor( ( (abs(12 - @{selected|EGO}) + (12 - @{selected|EGO})) / 2) / -6) ]]
```
## modLETAUX
```
[[ floor( ( (abs(12 - @{selected|LETAUX}) + (12 - @{selected|LETAUX})) / 2) / -3) ]]
```
## modMENTAL
```
[[ floor( ( (abs(12 - @{selected|MENTAL}) + (12 - @{selected|MENTAL})) / 2) / -3) ]]
```
## modNLETAUX
```
[[ floor( ( (abs(12 - @{selected|NLETAUX}) + (12 - @{selected|NLETAUX})) / 2) / -6) ]]
```

## Initiative
L'initiative verra le calcul automatiquement ajouté au tracker d'initiative si il est activé.
Le jet d'initiative comme lest autres doit se faire une fois le token sélectionné.
```
Initiative([[#D10 + @{selected|REF} + @{selected|INT} + #allmod &{tracker}]]) 
```

## Critical
le total d'un critique si le joueur décide re-rouer son 10 au lieu de faireune maneuvre
```
Total Critique ([[10 + 1D10!cs>10 ]]) 
```
## Image
```
[Image](?{Image URL|})
```
