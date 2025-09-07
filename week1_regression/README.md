# 📘 Week 1 - Régression

Nous présentons les **concepts théoriques de la régression** étudiés en Data Science.  

---

## 🌱 Qu’est-ce que la régression ?  

La **régression** est une méthode statistique et de machine learning qui permet de **modéliser** et **prédire** une variable cible (souvent notée **y**) en fonction d’une ou plusieurs variables explicatives (**features**, notées \(x_1, x_2, …, x_n\)).  

👉 En clair : c’est une façon de trouver la **relation** entre des données.  

**Exemple :** prédire la note d’un étudiant (y) en fonction du nombre d’heures d’étude (x).  

---

## 📘 1. Régression Linéaire  

- **Objectif :** prédire une **valeur continue** (salaire, prix, température).  
- **Modèle mathématique :**  

\[
y = \beta_0 + \beta_1 x_1 + \beta_2 x_2 + \dots + \beta_n x_n + \epsilon
\]

- \(y\) = valeur à prédire  
- \(x_i\) = variables explicatives  
- \(\beta_i\) = coefficients (impact de chaque variable)  
- \(\epsilon\) = erreur  

**Exemple :** prédire le **prix d’une maison** en fonction de sa surface et du nombre de chambres.  

---

## 📘 2. Régression Logistique  

- **Objectif :** prédire une **catégorie** (oui/non, malade/pas malade, spam/non-spam).  
- Utilise la **fonction sigmoïde** pour transformer la sortie en probabilité entre 0 et 1 :  

\[
P(y=1|x) = \frac{1}{1+e^{-(\beta_0 + \beta_1 x)}}
\]

- Si la probabilité > 0.5 → classe 1  
- Sinon → classe 0  

**Exemple :** prédire si un client va **résilier un abonnement** (1 = oui, 0 = non).  

---

## 📘 3. Régularisation  

Lorsque le modèle a beaucoup de variables, il peut trop bien mémoriser les données (**overfitting**).  
La régularisation ajoute une **pénalisation** pour contrôler les coefficients.  

- **Ridge (L2)** : réduit les grands coefficients (jamais à 0).  
- **Lasso (L1)** : pousse certains coefficients à 0 → sélectionne automatiquement les variables utiles.  
- **ElasticNet** : combinaison de L1 et L2.  

**Exemple :** prédire le salaire avec 50 variables (âge, ville, diplôme, …).  
Le Lasso peut ignorer les variables inutiles en mettant leurs coefficients à 0.  

---

## ✅ Résumé  

- **Régression linéaire** → prédire un **nombre** (valeur continue).  
- **Régression logistique** → prédire une **classe** (catégorie).  
- **Régularisation** → éviter le surapprentissage et simplifier le modèle.  

---

✍️ *Cours - Week 1 du parcours Data Science.*
