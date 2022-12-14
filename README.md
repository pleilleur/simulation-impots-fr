# Simulation du calcul d'imposition
Un simple tableur pour aider à comprendre le calcul des impôts et faire des simulations. Le [simulateur officiel](https://simulateur-ir-ifi.impots.gouv.fr/calcul_impot/2021/index.htm) fournit par impots.gouv.fr est utile et couvre d'autres cas de figure, mais il se remet à zéro à chaque simulation, il faut sccroller partout; pas super pratique.

# Ce qui est couvert

Les calculs sont effectués dans l'ordre suivant

1) Déduction/Abattement de 10%
2) Prise en compte des versements sur PER
3) Application de la CSG déductible de N-1
4) Application des parts
5) Calcul de l'imposition au barème IR avec le détail de chaque tranche
6) Décote
7) Déduction de la réduction d'impôts nette globale
8) Ajout des avances de crédit d'impôts
9) Déduction des avances (prélèvement à la source)

J'ai également couvert le cas des plus-values mobilières ou du revenu exceptionel (0XX). 

10) Application de la plus value au barème IR
11) Application de la plus value au PFU
12) Application d'un revenu exceptionnel, calcul au quotient
13) Calcul de la CSG déductible des plus-values pour N+1 

# Responsabilité

Il vous appartient de vérifier les règles en vigueur lors de votre déclaration, ce fichier vous permet de faire une simulation qui doit être confirmée par vos soins. Le résultat que vous obtiendrez n'est là qu'a titre informatif.

L'utilisation de ce fichier implique que vous connaissiez un minimum les sections concernées. Même si j'ai essayé de mettre des commentaires explicites, je ne peux pas couvrir les explications complètes de toutes les sections. 

# Versions

2022-08-12 - v4

- Correction du calcul de la CSG déductible de N-1
- Ajout du calcul de la CSG déductible des plus-values pour application en N+1

