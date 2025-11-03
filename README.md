# Politique de Confidentialité pour "Alias"

**Dernière mise à jour :** 3 novembre 2025

Nous vous remercions d'utiliser "Alias" (ci-après "l'Extension"). Votre vie privée est notre priorité absolue. Cette politique explique quelles données sont (et ne sont pas) traitées par l'Extension.

### 1. La Clé API

L'Extension nécessite que vous fournissiez votre propre clé API Google Gemini pour fonctionner.

* **Stockage :** Votre clé API est stockée **exclusivement sur votre machine locale** en utilisant l'API `chrome.storage.sync`.
* **Confidentialité :** Votre clé API n'est **jamais** envoyée à nos serveurs. Nous (les développeurs de l'Extension) n'y avons jamais accès. Elle n'est utilisée que pour communiquer directement de votre navigateur vers les serveurs de Google.

### 2. Données Traitées

L'Extension est conçue pour être un intermédiaire direct entre vous et l'API Gemini de Google.

* **Ce qui est envoyé à Google :** Lorsque vous utilisez l'Extension, deux éléments sont envoyés directement à l'API Google Gemini (`https://generativelanguage.googleapis.com`) :
    1.  Le **texte que vous avez sélectionné** sur la page.
    2.  Le **prompt (instruction) que vous avez rédigé** dans la fenêtre de l'Extension.
* **Objectif :** Ces données sont envoyées uniquement pour obtenir une réponse du modèle d'IA.
* **Ce qui n'est PAS envoyé :** L'Extension n'envoie aucune autre information, telle que votre historique de navigation, vos cookies, ou toute autre donnée personnelle.

### 3. Aucune Collecte de Données par l'Extension

C'est très simple : **"Alias" ne collecte, ne stocke, ne suit et ne vend AUCUNE donnée utilisateur.**

* Nous n'avons pas de serveurs pour collecter vos données.
* Nous n'utilisons aucun outil d'analyse (analytics).
* Nous ne surveillons pas la façon dont vous utilisez l'Extension.

Toute l'activité se déroule localement dans votre navigateur ou entre votre navigateur et l'API de Google, conformément à la [Politique de Confidentialité de Google](https://policies.google.com/privacy).

### 4. Permissions de l'Extension

L'Extension demande les permissions suivantes :

* **`storage` :** Pour stocker localement votre clé API Gemini et vos préférences de thème (clair/sombre).
* **`activeTab` / `<all_urls>` :** Pour détecter le texte que vous sélectionnez sur n'importe quelle page et afficher le bouton d'action.
* **`https://generativelanguage.googleapis.com/*` :** Pour autoriser l'Extension à envoyer des requêtes à l'API Gemini.
