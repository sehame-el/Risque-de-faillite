# Risque de Faillite - Analyse et Modélisation

## Description du projet

Ce projet s'inscrit dans le cadre d'un mémoire de Master en Économie Appliquée parcours Data Science à l'Université Paris-Est Créteil.

L'objectif principal de cette étude est d'identifier les facteurs influençant la défaillance des entreprises à partir de données économiques et financières. Le projet comprend une analyse exploratoire des données, la construction de modèles prédictifs ainsi que le développement d'une application permettant d'estimer le risque de faillite d'une entreprise en fonction de ses caractéristiques.

---

## Structure du projet

* `Mémoire.ipynb`: Notebook Jupyter contenant l'analyse complète, la modélisation, l'application Streamlit et l'interprétation des résultats.
* Les données utilisées ne sont pas incluses dans le dépôt pour des raisons de confidentialité.
* L'application Streamlit est lancée depuis le notebook directement.
* `README.md`: Documentation du projet.

---

## Utilisation

* Le notebook contient l'intégralité des étapes :

  * **Analyse exploratoire** : Visualisation des variables explicatives et corrélations.
  * **Préparation des données** : Nettoyage, transformation et normalisation.
  * **Modélisation** : Régression Logistique avec évaluation (ROC, Matrice de confusion).
  * **Application Streamlit** : Interface interactive pour estimer le risque de faillite.

⚠️ *Les données ne sont pas fournies dans le dépôt pour des raisons de confidentialité. L'application ne pourra pas fonctionner sans ces données.*

---

## Modélisation et Analyse

L'approche méthodologique adoptée est une **régression logistique** sur un ensemble de données provenant de **Crunchbase**. L'analyse se décompose en plusieurs étapes :

1. **Préparation et nettoyage des données :** Suppression des valeurs manquantes, normalisation et transformation des variables financières.
2. **Analyse descriptive et corrélationnelle :** Étude statistique des variables explicatives.
3. **Modélisation par régression logistique :** Estimation des paramètres et interprétation des coefficients.
4. **Évaluation des performances :**

   * Matrice de confusion
   * Courbe ROC (Receiver Operating Characteristic)
   * AUC (Area Under the Curve)

---

## Interprétation des résultats

### Importance des variables

D'après les résultats obtenus dans le mémoire, plusieurs variables ressortent comme influentes sur le risque de faillite :

* **Âge de l'entreprise** : Plus l'entreprise est ancienne, moins elle a de chances de faire faillite. Ce facteur est le plus significatif, indiquant que la stabilité acquise avec l'âge réduit les risques de défaillance.
* **Montant total des financements** : De manière contre-intuitive, un montant élevé de financement est associé à un risque plus important. Cela pourrait indiquer un besoin constant de liquidités pour compenser un modèle économique fragile.
* **Nombre de tours de financement** : Les entreprises ayant réalisé plusieurs levées de fonds semblent plus fragiles. Cela peut refléter une dépendance accrue au financement externe pour maintenir l'activité.
* **Secteur d'activité** : Les secteurs des semi-conducteurs et de la FinTech montrent un risque de faillite plus élevé, probablement en raison de la volatilité des marchés et de l'innovation technologique rapide.

### Profil d'une entreprise à risque

L'analyse montre qu'un profil type peut être identifié :

* Entreprises jeunes avec un fort montant de financement.
* Nombre de tours de financement élevés, indiquant un besoin constant de liquidité.
* Présence dans des secteurs plus volatils, tels que les semi-conducteurs et la FinTech.

Ces caractéristiques augmentent significativement les chances de fermeture.

### Limites du modèle

Le modèle présente certaines limites :

* Les données utilisées sont statiques et ne prennent pas en compte l'évolution temporelle des entreprises.
* L'absence de variables qualitatives (profil des dirigeants, stratégies de gestion) peut influencer la précision des prédictions.
* La réduction du statut à deux catégories (en activité ou fermée) ne permet pas d'identifier les entreprises en difficulté mais toujours actives.

---

## Application Prédictive

L'application **Streamlit** est directement intégrée dans le notebook. Lorsque le notebook est exécuté, l'application s'ouvre automatiquement dans le navigateur. Elle permet de :

* Saisir les caractéristiques d'une entreprise (âge, montants levés, secteur d'activité, etc.).
* Obtenir instantanément un score de probabilité de faillite.
* Visualiser un retour d'information sur les facteurs influents.

⚠️ *L'application nécessite les données pour fonctionner correctement. Elles ne sont pas incluses dans le dépôt.*

---

## Résultats principaux

* Les entreprises jeunes avec un fort montant de financement présentent un risque plus élevé.
* Les entreprises issues de certains secteurs (Semi-conducteurs, FinTech) montrent un risque plus important.
* L'âge de l'entreprise reste un facteur déterminant de stabilité.
* Le modèle est capable de détecter les entreprises à risque avec un bon niveau de précision.

---

## Améliorations possibles

* Intégration de données qualitatives (profil du dirigeant, stratégie d'entreprise).
* Utilisation de modèles plus avancés (Random Forest, XGBoost, etc.).
* Analyse temporelle pour capter l'évolution du risque dans le temps.
* Enrichissement des données pour améliorer la robustesse des prédictions.

---

## Contact

* **EL HACHMI Séhame**
* **Email :** lhmisehame@gmail.com

---

N'hésitez pas à me contacter pour toute question ou suggestion d'amélioration.
