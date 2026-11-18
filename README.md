<<<<<<< HEAD
# Analyse du Programme Social du Gouvernement (PSGouv 2)
### Réalisations 2023 – juin 2024 · Répartition territoriale et sectorielle

## Contexte

Le **PSGouv 2** est le programme social du gouvernement ivoirien. Ce projet
analyse la répartition de ses réalisations entre les **33 régions et districts**
du pays et les **6 grands secteurs** d'intervention (Éducative, Sanitaire,
Agricole, Électrique et Hydraulique, Sociale, Professionnelle).

**Question centrale** : *Comment les investissements sociaux du PSGouv 2 se
répartissent-ils entre les régions et les secteurs, et quelles disparités
territoriales peut-on identifier ?*

## Source des données

Dataset officiel « Réalisations du PSGouv 2 de 2023 à juin 2024 », publié sur
[data.gouv.ci](https://data.gouv.ci) — 1 337 lignes, 6 colonnes, 41 indicateurs.

## Démarche

1. **Inspection** : structure, typage, valeurs manquantes, doublons
2. **Diagnostic qualité** : détection de valeurs aberrantes (règle statistique
   > 10× la médiane) et d'incohérences métier (césarienne > accouchements,
   paludisme femme enceinte > total, etc.)
3. **Nettoyage documenté** : neutralisation de 38 valeurs corrompues (2,8 %),
   conservation de 97,2 % du dataset, traçabilité par colonnes de flags
4. **Analyse exploratoire** : couverture territoriale par secteur, top/flop
   régional sur 3 indicateurs phares, profil de l'Agnéby-Tiassa
5. **Dashboard interactif** (Power BI) — *en cours*

## Résultats clés

- **1 bug d'export systématique identifié** : 12 régions ont des valeurs
  corrompues sur 3 indicateurs de santé (CMU, césarienne, paludisme femme
  enceinte), confirmées par des incohérences logiques impossibles.
- **97,2 % des données conservées** après nettoyage documenté.
- **Le Sanitaire est le seul secteur universel** (couverture 68,8 %–100 %).
  L'Agricole est concentré sur 8 régions, le Professionnel est un programme
  pilote (17 régions).
- **Distribution proportionnelle à la population** : Abidjan domine les volumes
  absolus, concentration top 3 modérée (~32 %).
- **L'électrification est un programme rural** : BOUNKANI 1er (17,4 %),
  ABIDJAN 31e (0,2 %).
- **L'Agnéby-Tiassa est dans le premier quart** (rang médian 6/33), portée par
  la filière manioc.

## Limites méthodologiques

- Absence de données de population → pas de normalisation par habitant.
- Un 0 % de couverture ne distingue pas « programme absent » de « résultat nul ».
- Les montants FCFA ne sont pas agrégés avec les comptages (unités hétérogènes).
- Les 38 valeurs corrompues sont neutralisées, pas reconstituées.


## Auteur

**Franck Huberson KANGAH** — Master2 en Big Data Analytics
[GitHub](https://github.com/franckhuberson)
=======
# analyse_psgouv_v2
Le PSGouv 2 est le programme social du gouvernement ivoirien. Ce notebook analyse la répartition de ses réalisations entre les 33 régions et districts du pays et les 6 grands secteurs d'intervention (Éducative, Sanitaire, Agricole, Électrique et Hydraulique, Sociale, Professionnelle).
>>>>>>> 827354dce80c0b9ac7cf4a583db21f601fe8fe19
