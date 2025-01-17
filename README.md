# ZONE_LA_PLUS_CHAUDE_EN_FRANCE_DE_2000-2009


### ✍️ Auteurs
- **Anis Ghouas**
- **Alio Hissein Alio**
- **Groupe : Shannon**

Année universitaire : **2024-2025**
# 🌡️ Détermination des zones les plus chaudes

## 📖 Introduction
Ce projet, développé dans le cadre de **SAE 105 : Traitement des données**, a pour objectif principal d’identifier les zones géographiques les plus chaudes à partir de données météorologiques détaillées. Il offre une analyse personnalisable en fonction de la période choisie, de la résolution temporelle, et du type de zone (station ou coordonnées géographiques).  
Grâce à ce projet, nous avons exploré des techniques de manipulation et d’analyse de données climatiques, ainsi que leur interprétation pour en tirer des informations utiles.

---

## 🎯 Objectifs du projet
1. Traiter de grandes quantités de données climatiques provenant de fichiers CSV.
2. Analyser les températures maximales en fonction d’une période et d’une résolution spatiale définies par l'utilisateur.
3. Permettre une personnalisation de l’analyse grâce à des paramètres :
   - **Durée** : Période d’analyse sélectionnée par l’utilisateur.
   - **Résolution temporelle** : Choix entre une analyse horaire, journalière, mensuelle ou annuelle.
   - **Type de zone** : Analyse par station météorologique ou par coordonnées géographiques.
4. Identifier et afficher la région ou la station ayant enregistré la température la plus élevée.

---

## 🗂️ Structure des données

Les fichiers utilisés pour ce projet contiennent des données météorologiques fournies par Météo-France. Voici les principales colonnes et métadonnées contenues dans les fichiers CSV :

| **Champ**       | **Description**                                                                                              | **Unité**                   |
|------------------|------------------------------------------------------------------------------------------------------------|-----------------------------|
| **NUM_POSTE**    | Numéro unique de la station météorologique (8 chiffres).                                                   | -                           |
| **NOM_USUEL**    | Nom usuel de la station météorologique.                                                                    | -                           |
| **LAT**          | Latitude de la station (valeurs négatives au sud).                                                         | Degrés et millionièmes      |
| **LON**          | Longitude de la station (valeurs négatives à l’ouest de Greenwich).                                        | Degrés et millionièmes      |
| **ALTI**         | Altitude de la station.                                                                                    | Mètres                      |
| **AAAAMMJJHH**   | Date et heure de la mesure.                                                                                | Format `YYYYMMDDHH`         |
| **T**            | Température enregistrée (ou `"mq"` si donnée manquante).                                                  | °C                          |
| **PMERM**        | Moyenne quotidienne des pressions au niveau de la mer.                                                    | hPa (1/10)                  |
| **INST**         | Durée d’ensoleillement quotidienne.                                                                        | Minutes                     |
| **UV_INDICEX**   | Maximum des indices UV horaires.                                                                           | -                           |

### 🔍 Gestion des données manquantes
- Les températures marquées comme `"mq"` sont automatiquement ignorées dans le traitement.
- Les lignes malformées ou contenant des incohérences sont également passées pour garantir l’exécution du programme.

---

## 🛠️ Fonctionnalités du projet
1. **Lecture et traitement des fichiers CSV** : Extraction des données climatiques pour les stations ou zones géographiques.
2. **Personnalisation de l’analyse** :
   - Choix de la période d’analyse via des dates de début et de fin.
   - Sélection de la résolution temporelle (heure, jour, mois ou année).
   - Possibilité d’analyser les données par station.
3. **Calcul des statistiques** :
   - Nombre total de relevés pour chaque région.
   - Température maximale enregistrée.
   - Température moyenne pour chaque région.
4. **Identification de la région ou station la plus chaude** :
   - Région ayant enregistré la température maximale pendant la période analysée.
   - Affichage de la température maximale correspondante.

---

###  Conclusion
Grâce à ce projet, nous avons pu maîtriser les techniques de traitement et d’analyse de données climatiques, tout en répondant à des problématiques concrètes comme l’identification des zones les plus chaudes. Les résultats obtenus démontrent la flexibilité et la précision des outils mis en œuvre.
