Notebook interactif pour prédire le risque de départ d'un collaborateur en fonction de sa satisfaction et ancienneté.

🎯 À quoi ça sert ?
Pour RH / managers PME :

Estimer rapidement le risque turnover d'un collaborateur

Identifier les signaux faibles avant démission

Décision data-driven : qui prioriser pour entretien / plan de carrière ?

Exemple : Satisfaction 3/10 + 1 an d'ancienneté = 95% risque départ 🟠

📊 Comment ça marche
Données d'entraînement (8 collaborateurs)
Satisfaction	Ancienneté	Risque départ
8	5 ans	10% 🟢
3	1 an	80% 🔴
...	...	...
Modèle
Régression linéaire simple :

text
risque = 1.073 - (0.098 × satisfaction) - (0.021 × ancienneté)
Sliders interactifs :

Satisfaction : 1-10

Ancienneté : 1-15 ans

Résultat instantané avec code couleur (🟢🟠🔴)

🚀 Utilisation
Ouvrir Colab : Lien direct

Glisser sliders pour tester profils

Copier formule pour Excel / SIRH

💾 Exemples résultats
text
👉 Satisfaction 7 + 8 ans = 22% 🟢 Risque FAIBLE
👉 Satisfaction 4 + 2 ans = 72% 🔴 Risque ÉLEVÉ
👉 Satisfaction 5 + 5 ans = 49% 🟠 Risque MODÉRÉ
🔧 Personnalisation
python
# Ajouter tes données réelles
data = {
  'satisfaction': [tes_valeurs],
  'ancienneté':   [tes_valeurs],
  'risque_départ':[tes_valeurs_réelles]
}
📈 Pourquoi ce modèle ?
Simplicité : 2 variables, 1 formule

Interprétable : coefficients lisibles

PME-friendly : pas de data scientist requis

Actionnable : risque chiffré + couleur

🤝 Crédits
DataRH - Consulting Data RH pour PME
competencesrh.fr/data-ia-rh.html
