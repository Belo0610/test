# FalconServer

![FalconServer Logo](https://cosiest-cichlid-3505.dataplicity.io/FalconServer.png)

FalconServer est un système d'hébergement de sites web directement depuis votre PC ou téléphone. Il est performant, personnalisable et facile à utiliser.

## 🚀 Fonctionnalités
- Hébergement de sites web en **HTML, CSS, JavaScript** avec prise en charge du **Python** via les balises `<py>`(attention: on ne peus pas inporter de modules python dans les page web)
- Configuration simplifiée avec un fichier `config/config.yml`
- Gestion des logs détaillés (IP, date, heure, requêtes...)
- Pages d'erreur personnalisables
- Léger, rapide et optimisé pour toutes les plateformes

## 📦 Installation
### 1. Téléchargement du projet
windows
```bash
Invoke-WebRequest -Uri "https://cosiest-cichlid-3505.dataplicity.io/installer_de_FalconServer.py" -OutFile "installer_de_FalconServer.py"; python installer_de_FalconServer.py
```
linux
```bash
wget https://cosiest-cichlid-3505.dataplicity.io/installer_de_FalconServer.py && python3 installer_de_FalconServer.py 
```
### 2. Configuration
Modifiez le fichier `config/config.yml` selon vos préférences :
```yaml
# Configuration principale
0.0.0.0: true          # Autoriser les connexions depuis toutes les adresses IP
localhost: true        # Autoriser les connexions depuis localhost
port: 8080             # Port sur lequel le serveur écoutera

# Configuration des pages d'erreur
error_pages:
  404: "404.html"      # Page d'erreur pour 404 (page non trouvée)
  500: "500.html"      # Page d'erreur pour 500 (erreur interne)
  403: "403.html"      # Page d'erreur pour 403 (accès interdit)

# Paramètres supplémentaires
get_ip: true           # Activer ou désactiver les logs des adresses IP


```

### 3. Lancement du serveur
```bash
python3 falconserver.py
```

## 🔧 Personnalisation
Vous pouvez modifier les pages d'erreurs et ajuster les paramètres du serveur via `config/config.yml`. FalconServer prend en charge les fichiers HTML et l'intégration Python avec `<py>`.

## 🛠 Dépendances
- **Python 3.x**
- **Bibliothèques requises** (installées automatiquement) :
  ```bash
  pip install -r requirements.txt
  ```


## 🤝 Contribuer
Les contributions sont les bienvenues ! N'hésitez pas à ouvrir une issue ou à soumettre une pull request.

## 📢 Contact
- **Créé par** : Belo (<@1187484890795622471>)
- **Discord** : [Rejoindre FalconStudios](https://discord.gg/BD7NUbHJYG)

---
✨ *FalconServer – L'hébergement web simplifié.*

