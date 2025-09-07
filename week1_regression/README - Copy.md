# Régression - Machine Learning Classique

## 🎯 Objectifs
- Comprendre et appliquer la **régression linéaire** (simple et multiple)
- Découvrir la **régression logistique** (binaire et multiclasse)
- Appliquer les techniques de **régularisation** : Ridge, Lasso, ElasticNet
- Utiliser **Scikit-learn** pour entraîner, évaluer et comparer des modèles
- Réaliser un **mini-projet** de prédiction du prix des maisons

---

## 📖 Concepts Théoriques

### 1. Régression Linéaire
- Modèle pour prédire une variable continue :  
\[
y = \beta_0 + \beta_1 x_1 + \beta_2 x_2 + ... + \beta_n x_n + \epsilon
\]
- Objectif : approximer la relation entre **features** et **target**.
- Utilisations : prédiction du prix d’une maison, prévision de ventes, etc.

### 2. Régression Logistique
- Sert à prédire une **classe** (0/1 ou multiclasse) à partir des features.  
- Fonction sigmoïde :  
\[
P(y=1|x) = \frac{1}{1+e^{-(\beta_0 + \beta_1 x)}}
\]  
- Exemples : prédire si un client va churner, survie d’un passager Titanic.

### 3. Régularisation
- Évite le **surapprentissage** (overfitting) sur des datasets avec beaucoup de variables.  
- **Ridge (L2)** : pénalise les grands coefficients  
- **Lasso (L1)** : pousse certains coefficients à 0 (sélection de variables)  
- **ElasticNet** : combinaison de L1 et L2

---

## ⚙️ Scikit-learn API
| Modèle | Classe Scikit-learn |
|--------|------------------|
| Régression linéaire | `LinearRegression()` |
| Régression logistique | `LogisticRegression()` |
| Ridge | `Ridge()` |
| Lasso | `Lasso()` |
| ElasticNet | `ElasticNet()` |

---

## 📝 Mini-Projet : Prédiction du Prix des Maisons
- **Dataset** : Boston Housing (`sklearn.datasets`) ou Kaggle House Prices
- **Étapes recommandées** :
1. Charger et explorer les données (`pandas`, `head()`, `describe()`)  
2. Prétraitement : nettoyage, normalisation, séparation train/test  
3. Entraîner plusieurs modèles : LinearRegression, Ridge, Lasso  
4. Évaluer avec **RMSE** et **R²**  
5. Visualiser les résultats (scatter plots, courbes prédiction vs réalité)  

- **Extensions possibles** :
  - Tester ElasticNet et comparer aux autres modèles  
  - Sélection de features importantes avec `coef_`  
  - GridSearchCV pour tuning hyperparamètres

---

## 📚 Ressources
- Aurélien Géron – *Hands-On Machine Learning with Scikit-Learn & TensorFlow*, Chapitre 4  
- [Scikit-learn Linear Models Documentation](https://scikit-learn.org/stable/modules/linear_model.html)  
- [Kaggle House Prices Dataset](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)  

---

## 🚀 Instructions pour exécuter les notebooks
1. Installer les packages nécessaires :  
```bash
pip install numpy pandas matplotlib scikit-learn

