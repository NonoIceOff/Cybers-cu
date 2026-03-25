# Politique de sécurité mobile et de développement

## 1. Usage des appareils

- L'entreprise fournit des téléphones professionnels et l'utilisation de téléphones personnels est interdite pour garantir la confidentialité des données sensibles.
- Pas d'installation d'applications depuis les boutiques publiques sur les téléphones professionnels. Seules les applications nécessaires au travail doivent être téléchargées via le site officiel de l'entreprise.

## 2. Sécurité et gestion des appareils

- Chaque téléphone professionnel doit être protégé par un code PIN fourni par l'entreprise qui ne doit jamais être désactivé.
- Les appareils professionnels sont gérés via un MDM (Mobile Device Management) permettant le contrôle et la sécurité centralisés.

## 3. Mise à jour des appareils

- Il est obligatoire de maintenir tous les téléphones et PC professionnels à jour avec les dernières versions logicielles et patchs de sécurité.

## 4. Sauvegarde des projets

- Tous les projets doivent être régulièrement sauvegardés sur les systèmes de stockage de l'entreprise pour éviter la perte de données.

## 5. Politique de développement sécurisé

En complément des mesures de sécurité mobile, une politique de développement sécurisée doit être respectée pour limiter les vulnérabilités identifiées lors des audits :

- **Protection des clés et secrets** : ne jamais stocker les clés API, identifiants Firebase ou secrets en clair dans le code ou les fichiers de configuration (ex : strings.xml). Utiliser des mécanismes sécurisés côté serveur.
- **Stockage sécurisé** : les données sensibles ne doivent jamais être stockées en Base64 ou en clair dans SharedPreferences. Utiliser un chiffrement robuste et validé.
- **Certificate pinning** : utiliser des algorithmes de hachage modernes (SHA-256 ou supérieurs) et maintenir les pins à jour pour éviter de revenir à la confiance système.
- **Transmission des données** : toutes les communications réseau doivent être chiffrées et le trafic en clair est strictement interdit.
- **Gestion des cookies et sessions** : éviter la persistance locale de cookies contenant des informations de session sensibles, et s'assurer que leur stockage est sécurisé.
- **Séparation des couches** : les identifiants et mots de passe ne doivent jamais être transmis en clair entre la couche native et React Native ou toute autre couche applicative.
- **Revue de code et audits réguliers** : mettre en place des revues de code systématiques et des audits de sécurité réguliers pour détecter les failles comme celles identifiées (padding oracle, endpoints exposés, API keys visibles).

Cette politique vise à renforcer la sécurité des applications mobiles et à protéger les données sensibles de l'entreprise ainsi que celles des clients.
