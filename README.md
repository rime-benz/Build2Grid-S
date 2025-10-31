# Build2Grid-S : Paramètres du Modèle de Raccordement
# ⚡ Build2Grid --- Smart Electrification Planning

> **Build2Grid** optimise le raccordement électrique des bâtiments en
> combinant SIG, Python et une logique de priorisation intelligente
> (coût, distance, densité, criticité hospitalière).

------------------------------------------------------------------------

## 🎯 Objectifs

-   ⚡ Raccorder efficacement un territoire au réseau électrique
-   🏥 Prioriser les **sites critiques** (hôpital en phase 0)
-   📊 Maximiser les **logements raccordés tôt**
-   💰 Respecter budget & capacité terrain
-   🧠 Exploiter une **métrique dynamique** 
-   📍 Automatisation SIG (QGIS + Python)

------------------------------------------------------------------------

## 🧠 Modèle Build2Grid‑S --- Paramètres du raccordement

  Paramètre                Valeur / Rôle
  ------------------------ ---------------------------------------------------------
  Types d'infrastructure   Aérien / Semi‑aérien / Fourreau
  Coûts                    500 €/m --- 750 €/m --- 900 €/m
  Temps d'installation     2h/m --- 4h/m --- 5h/m (4 ouvriers max)
  Coût main‑d'œuvre        300 €/jour / ouvrier
  Site critique            Hôpital (autonomie 20h → intervention ≤ 16h ✅)
  Critères                 Distance réseau, nb logements, surface, puissance, zone

------------------------------------------------------------------------

## 🚦 Phasage du raccordement

  Phase     Cible                   Logements   Progression             Budget
  --------- --------------------- ----------- ------------- ------------------
  Phase 0   Hôpital                    1 site           ---   Priorité absolue
  Phase 1   Haute densité                                                  40%
  Phase 2   Services publics                                               20%
  Phase 3   Maisons diffuses                                                20%
  Phase 4   Finalisation réseau                                              20%

------------------------------------------------------------------------

## 🗂️ Architecture du projet

    Build2Grid/
     ├── data/
     │   ├── batiments.csv
     │   ├── infra.csv
     ├── scripts/
     │   └── Script_optimisation.ipynb
     ├── outputs/
     │   ├── graphs/
     │   └── reports/
     └── README.md

------------------------------------------------------------------------

## ▶️ Exécution

``` bash
jupyter notebook Script_optimisation.ipynb
```

------------------------------------------------------------------------

## 📊 Sorties générées

-   ✅ Tableaux phases & logements
-   ✅ Graphiques progression & répartition réseau
-   ✅ Carte QGIS
-   ✅ Rapport automatisé **Word + PDF**

------------------------------------------------------------------------

## 🚀 Améliorations futures

-   🌄 Prise en compte du relief
-   👷 Multi‑équipes + diagramme Gantt
-   🌐 Interface web interactive
-   🤖 IA : suggestion automatique de tracé réseau

------------------------------------------------------------------------

## © Licence

Projet Build2Grid --- 2025\
Open collaboration --- contribution bienvenue !
