# 🥦 Projet Data Governance — Open Food Facts

## 📌 Contexte
Ce projet simule une mission de **Data Steward** sur un dataset réel et public : 
la base Open Food Facts, qui recense les produits alimentaires vendus dans le monde.

L'objectif est de démontrer les compétences clés en gouvernance de la donnée : 
documentation, audit qualité et visualisation.

---

## 🎯 Objectifs
- Construire un **Data Dictionary** complet sur 12 champs
- Réaliser un **audit de qualité** des données (taux de complétude, anomalies)
- Produire un **dashboard Power BI** avec des insights métier

---

## 📦 Dataset
- **Source** : [Open Food Facts](https://world.openfoodfacts.org/) via Kaggle
- **Périmètre** : Produits vendus en France uniquement
- **Volume** : 112 171 produits · 12 champs sélectionnés

---

## 🛠️ Outils utilisés
| Outil | Usage |
|---|---|
| Terminal (Mac) | Extraction et filtrage du dataset |
| Google Sheets | Data Dictionary + Audit Qualité |
| Power BI | Dashboard de visualisation |
| GitHub | Documentation et partage |

---

## 📋 Data Dictionary
12 champs documentés avec type, description métier, exemple et règle de qualité.

| Champ | Type | Description |
|---|---|---|
| product_name | Texte | Nom commercial du produit |
| brands | Texte | Marque commerciale |
| categories | Texte | Catégorie alimentaire |
| countries | Texte | Pays de vente |
| ingredients_text | Texte | Liste des ingrédients |
| additives_n | Nombre entier | Nombre d'additifs |
| nutrition_grade_fr | Texte | Nutri-Score (A à E) |
| energy_100g | Nombre décimal | Énergie pour 100g (kcal) |
| fat_100g | Nombre décimal | Matières grasses pour 100g |
| sugars_100g | Nombre décimal | Sucres pour 100g |
| salt_100g | Nombre décimal | Sel pour 100g |
| last_modified_t | Date | Date de dernière modification |

---

## 📊 Résultats de l'audit qualité

| Champ | Taux de complétude | Statut |
|---|---|---|
| last_modified_t | 100% | 🟢 Bon |
| product_name | 98,89% | 🟢 Bon |
| brands | 98,34% | 🟢 Bon |
| countries | 100% | 🟢 Bon |
| ingredients_text | 76,65% | 🟡 Moyen |
| additives_n | 76,66% | 🟡 Moyen |
| nutrition_grade_fr | 82,58% | 🟡 Moyen |
| energy_100g | 85,55% | 🟡 Moyen |
| fat_100g | 71,67% | 🔴 Critique |
| sugars_100g | 83,94% | 🟡 Moyen |
| salt_100g | 83,99% | 🟡 Moyen |
| categories | 67,81% | 🔴 Critique |

---

## 💡 Insights clés
- Le Nutri-Score **D** est le plus fréquent parmi les produits français
- Les champs nutritionnels ont un taux de complétude moyen de **~80%**
- Les produits avec Nutri-Score **D et E** contiennent plus d'additifs en moyenne
- **categories** et **fat_100g** sont les champs les plus critiques à améliorer

---

## 📁 Structure du projet
