##### Deux solutions MDM :

* Microsoft Intune
* NinjaOne





##### Microsoft Intune

Solution MDM intégrée au Microsoft 365 et Azure AD qui propose une gestion centralisée des appareils, des politiques de conformité et une sécurité renforcée. Elle prend en charge iOS, Android, Windows et macOS, permet des déploiements à grande échelle, des politiques d’accès conditionnel, le chiffrement, la suppression à distance et une intégration étroite avec les services Microsoft (Word, Excel, etc...).

###### Avantages :

* Forte intégration avec l’écosystème Microsoft (Azure AD, Defender, M365)
* Large couverture multiplateforme (prend en charge les OS les plus utilisés)
* Capacités de sécurité et conformité avancées

###### Inconvénients :

* Mise en place initiale complexe
* Coût élevé pour les petites organisations





##### NinjaOne

Solution MDM robuste orientée gestion des appareils mobiles avec une plateforme unifiée permettant de gérer Android, iOS et autres terminaux depuis un seul tableau de bord. Elle propose une gestion centralisée des appareils, une fonctionnalité de déploiement des applications, des politiques à grande échelle, une gestion de verrouillage/effacement à distance et de restriction des fonctions des appareils pour renforcer la conformité et la sécurité.

###### Avantages :

* Grande compatibilité des appareils (Android et Apple) et gestion unifiée sur une seule plateforme avec surveillance, politiques et actions centralisées.
* Fonctions de sécurité fortes avec verrouillage, effacement à distance, réinitialisation de code d’accès et restrictions des fonctionnalités.
* Déploiement et enrôlement rapides des appareils, avec gestion des applications et des stratégies sur toute la flotte.

###### Inconvénients :

* Les fonctionnalités avancées peuvent être perçues comme complexes pour des équipes très restreintes ou sans expérience MDM.
* Solution intégrée à une plateforme plus large, ce qui peut nécessiter une adaptation ou formation pour exploiter pleinement toutes les capacités.





##### Tableau comparatif

|Catégories|Microsoft Intune|NinjaOne (MDM)|
|-|-|-|
|**Architecture**|Cloud Microsoft Natif|Saas cloud unifié|
|**Gestion des Identités**|Intégration native et profonde avec Microsoft Azure.|Intégration via connecteurs, mais orientée gestion de flotte par terminaux.|
|**Déploiement**|Autopilot (Windows), Apple Business Manager (ADE), Android Enterprise.|Via portail, QR code ou intégration Apple/Google.|
|**Sécurité**|Accès conditionnel (ex: interdire Outlook si l'OS n'est pas à jour).|Verrouillage, effacement à distance et réinitialisation de code ultra-rapides.|
|**Gestion applicative**|Déploiement granulaire (MAM) : Word, Excel, etc., avec protection des données internes.|Distribution d'apps simplifiée et gestion des politiques sur toute la flotte en masse.|
|**Facilité d'usage**|Complexe : nécessite des compétences pour une bonne configuration.|Facile : interface moderne, prise en main rapide même sans compétences particulières.|
|**Points forts**|Intégration totale avec la suite Office|Déploiement rapide|
|**Inconvénients**|Interface lourde pour de petites tâches|Contrôle limité sur les applications|



