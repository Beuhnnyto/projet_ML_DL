# 🏠 Projet ML - Prédiction des Prix Immobiliers à Paris

## 📋 Description

Projet d'apprentissage automatique visant à analyser et prédire les prix immobiliers à Paris en utilisant les transactions DVF (Données de Valeur Foncière) issues de **Data.gouv**.

**Objectif métier** : Construire un modèle robuste pour expliquer et prédire le **prix au m²** des appartements parisiens, en fonction des caractéristiques du bien et de la localisation.

---

## 📂 Structure du Projet

```
projet_ML_DL/
├── README.md                              # Ce fichier
├── projet_immobilier_paris_eda.ipynb     # Notebook principal (EDA)
└── data/                                  # Données téléchargées (généré à l'exécution)
```

---

## 🎯 Étapes Couvertes (Actuel)

- ✅ **1. Problème** : contexte métier et objectifs
- ✅ **2. Données** : source DVF, description, limitations
- ✅ **3. Analyse Exploratoire (EDA)** : visualisations, insights clés, clustering exploratoire

## 📋 Étapes à Venir (Sections 4-8)

- ⏳ **4. Préparation** : pipeline sklearn, gestion NA, encodage
- ⏳ **5. Modélisation** : Linear Regression, Random Forest, Gradient Boosting
- ⏳ **6. Évaluation** : métriques (MAE, RMSE, R²), validation croisée
- ⏳ **7. Analyse** : interprétation des résultats
- ⏳ **8. Conclusion** : recommandations et travaux futurs

---

## 🚀 Démarrage Rapide

### Prérequis
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### Lancer le Notebook

1. Ouvrir le notebook Jupyter
2. Exécuter les cellules **séquentiellement**
3. Le notebook télécharge automatiquement les données DVF

```bash
jupyter notebook projet_immobilier_paris_eda.ipynb
```

---

## 📊 Source de Données

**Provenance** : Geo-DVF - Data.gouv (transactions immobilières françaises)

| Année | URL |
|-------|-----|
| 2022 (principal) | `https://files.data.gouv.fr/geo-dvf/latest/csv/2022/departements/75.csv.gz` |
| 2021 (fallback) | `https://files.data.gouv.fr/geo-dvf/latest/csv/2021/departements/75.csv.gz` |

**Filtrage appliqué** :
- Type de mutation : **Ventes uniquement**
- Type de local : **Appartements**
- Commune : **Paris (75)**
- Nettoyage : suppression des valeurs invalides et outliers extrêmes (1%-99%)

---

## 📌 Points Clés EDA

Après exécution du notebook, complétez cette section avec vos observations :

- Distribution du prix au m² (histogramme, asymétrie)
- Variation géographique par arrondissement
- Corrélations entre surface, prix total et prix au m²
- Segments de marché (clusters non supervisés)
- Tendances temporelles

---

## 📝 Notes Importantes

- **Pas de fuite de données** : le pipeline train/test sera implémenté dans la phase 4
- **Données publiques** : aucune donnée sensible, usage libre
- **Outliers** : conservés dans l'EDA pour analyse, seront gérés proprement au nettoyage

---

## 👥 Équipe & Contact

*À compléter avec vos informations*

---

## 📄 Licence

Données DVF publiques (licence ODbL 1.0, Data.gouv)\n