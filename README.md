# HealthEstim – Simulateur éthique de frais médicaux

## Structure du projet
```
├── app.py               # Application Streamlit principale
├── requirements.txt     # Dépendances Python
├── insurance_data.csv   # Dataset (anonymisé pour le modèle)
├── model_lr.pkl         # Modèle Régression Linéaire entraîné
├── feature_cols.json    # Colonnes du modèle
└── app.log              # Journaux (généré automatiquement)
```

## Lancement local
```bash
pip install -r requirements.txt
streamlit run app.py
```

## Déploiement Streamlit Cloud
1. Créer un repo GitHub avec ces fichiers
2. Aller sur https://share.streamlit.io
3. Connecter le repo → sélectionner `app.py`
4. Déployer → URL publique HTTPS générée automatiquement

## Comptes de démo
| Utilisateur | Mot de passe | Rôle |
|-------------|-------------|------|
| admin       | admin123    | Admin (accès logs) |
| demo        | demo2024    | Utilisateur standard |

## Conformité RGPD
- Aucune donnée PII dans le modèle (NSS, email, IP, nom/prénom exclus)
- Bannière consentement à la connexion
- Logs sans données personnelles
- Simulation locale (aucune persistance)

## Accessibilité WCAG AA
1. Contrastes ≥ 4.5:1 (texte sur fond)
2. Navigation clavier avec focus visible
3. Attributs ARIA sur composants dynamiques
