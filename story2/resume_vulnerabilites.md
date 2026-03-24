### Status en DANGEROUS

###### L’application présente des risques de sécurité importants. Elle demande des permissions sensibles qui peuvent exposer des données personnelles ou permettre des actions non sécurisées comme la lecture des contacts, et surtout l'écriture en dehors du scope de l'application (non necessaire, et très dangereux)



* android.permission.READ\_CONTACTS
* android.permission.WRITE\_EXTERNAL\_STORAGE



### 

### Problèmes de manifest :

###### L’application peut être installée sur des versions anciennes d’Android et donc peut être installée sur des versions vulnérables. De plus, les données sont envoyés et reçus sans cryptage (mots de passe, emails, autres données sensibles), ce qui est pas terrible.



* App can be installed on a vulnerable unpatched Android version 4.4-4.4.4, \[minSdk=19]
* Clear text traffic is Enabled For App\[android:usesCleartextTraffic=true] 







### CODE ANALYSIS

###### Le chiffrement utilisé repose sur le mode CBC avec un padding PKCS5/PKCS7, une configuration vulnérable à certaines attaques comme les padding oracle, ce qui peut compromettre la confidentialité des données.



* The App uses the encryption mode CBC with PKCS5/PKCS7 padding. This configuration is vulnerable to padding oracle attacks.







### FIREBASE :

###### Firebase Remote Config est activé et accessible via une API publique. Des personnes pourraient regarder la structure du projet, et connaître donc la structure du projet.



* Firebase Remote Config enabled	warning	The Firebase Remote Config at https://firebaseremoteconfig.googleapis.com/v1/projects/717748501407/namespaces/firebase:fetch?key=AIzaSyBTgztvImsUfMWDa41PCrDWAj7dmyIDhUg is enabled. Ensure that the configurations are not sensitive. This is indicated by the response: {'entries': {'APP\_VERSION\_SUPPORT\_BENEFICIARY\_ADDING': ''}, 'state': 'UPDATE', 'templateVersion': '60'}



