# RollQuery pour un jet d'esprit

Permet un jet de dées et calcul automatiquement 

* Le modificateur de blessures Letal, non Letal, mental, ego et fatigue (chi)
* Ajoute le modificateur d'esprit
* Ajoute le modificateur de la skill
* Roule le dé (selon la macro [D10](./ensemble-base.macroset.md#D10))

```javascript
?{Esprit|
Esprit        ,Esprit         ([[#D10 + #allmod + [[@{selected|ESP}]] + [[0]]                          ]]) |
Astrogation  ,Astrogation   ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|Astrogation}]]   ]]) |
Bureaucratie  ,Bureaucratie   ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|Bureaucratie}]]   ]]) | 
Chi(Yang)     ,Chi(Yang)      ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|ChiYang}]]        ]]) |
Communication ,Communication  ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|Communication}]]        ]]) |
Dissimulation ,Dissimulation  ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|Dissimulation}]]  ]]) |
Fouille       ,Fouille        ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|Fouille}]]        ]]) |
Guérison      ,Guérison       ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|Guérison}]]       ]]) |
Ingénerie     ,Ingénerie      ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|Ingénerie}]]      ]]) |
Jeux          ,Jeux           ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|Jeux}]]           ]]) |
Lire et Écrire,Lire et Écrire ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|LireÉcrire}]]     ]]) |
Mécanisme     ,Mécanisme      ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|Mécanisme}]]      ]]) |
Mécanique     ,Mécanique      ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|Mécanique}]]      ]]) |
Médecine      ,Médecine       ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|Médecine}]]       ]]) |
Musique       ,Musique        ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|Musique}]]        ]]) |
Navigation    ,Navigation     ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|Navigation}]]     ]]) |
Pistage       ,Pistage        ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|Pistage}]]        ]]) |
Premier Soins ,Premier Soins  ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|PremierSoins}]]   ]]) |
Programmation ,Programmation  ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|Programmation}]]   ]]) |
Region(Song)  ,Region(Song)   ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|Region_Song}]]    ]]) |
Survie        ,Survie         ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|Survie}]]         ]]) |
Système planétaire ,Système planétaire ([[#D10 + #allmod + [[@{selected|ESP}]] + [[%{selected|Systèmeplanétaire}]]  ]]) |
}&{v1.0.0}&{noerror} = D$[[0]] + mod$[[6]] + @$[[7]] + sk$[[8]]
```
