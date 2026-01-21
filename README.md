# 🎖️ Legion PDF Editor

Une solution web légère et élégante pour visualiser et éditer le texte de vos fichiers PDF. Ce projet utilise une architecture hybride : une interface frontend hébergée sur **GitHub Pages** et un moteur de traitement Python via un tunnel **Cloudflare**.

## 🚀 Fonctionnalités

* **Visualisation native** : Lisez vos PDF directement dans le navigateur.
* **Édition de texte** : Convertissez vos PDF en texte éditable, modifiez-les et régénérez un nouveau PDF.
* **Interface Moderne** : Design fluide avec modes Grille et Liste, optimisé pour ordinateur.
* **Zéro Installation** : Pour l'utilisateur final, tout se passe dans le navigateur.

## 🛠️ Installation & Configuration

### 1. Le Serveur (Backend)
Le site a besoin de son "moteur" pour fonctionner. Assurez-vous que votre serveur Python est actif :
1. Lancez votre script `main.py` (ou le nom de votre API).
2. Activez le tunnel Cloudflare pour obtenir l'URL publique.

### 2. Le Site (Frontend)
Le frontend est configuré pour pointer vers votre URL Cloudflare.
* Fichier principal : `index.html`
* Hébergement : GitHub Pages

## 📖 Comment l'utiliser ?

1.  Ouvrez le lien du site généré par GitHub Pages.
2.  Cliquez sur le bouton **+** pour importer un PDF.
3.  Cliquez sur le document pour ouvrir le menu d'actions.
4.  **Lire** : Ouvre le PDF dans la visionneuse.
5.  **Éditer** : Envoie le PDF au serveur pour extraction du texte, permet la modification, puis propose le téléchargement du nouveau PDF.

## ⚠️ Notes Importantes

* **Connexion au serveur** : Si le bouton "Éditer" ne répond pas, vérifiez que l'URL `API_URL` dans le fichier `index.html` correspond bien à votre tunnel Cloudflare actuel.
* **Confidentialité** : Les fichiers sont traités temporairement par votre serveur local pour la conversion.

---
