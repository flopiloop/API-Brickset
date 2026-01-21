# SAE 3.VCOD.01 - Brickset API Explorer

Application Python interfacée avec l'API Brickset pour explorer et gérer des collections LEGO. L'outil permet d'interroger des sets, de gérer des collections personnelles via une interface terminal, et de générer automatiquement une galerie web structurée des sets.

## Fonctionnalités

- **Recherche de sets LEGO** : Interrogation de l'API Brickset par thème, année ou ID de set
- **Interface terminal interactive** : Menu en ligne de commande pour naviguer facilement
- **Génération de galerie web** : Export automatique en HTML/CSS des collections

## Installation

1. Cloner le dépôt :
```bash
git clone https://github.com/flopiloop/API-Brickset.git
cd API-Brickset
```

2. Installer les dépendances :
```bash
pip install -r requirements.txt
```

3. Configurer l'API :
```bash
cp .env.example .env
# Éditer .env avec votre clé API Brickset
```

Vous pouvez obtenir une clé API gratuite sur [Brickset](https://brickset.com/tools/webservices/requestkey).

## Utilisation

```bash
cd src
python main.py
```

Les fichiers générés seront disponibles dans le dossier `DATA/`.

## Structure du projet

```
SAE_terminée/
├── src/
│   ├── main.py        # Point d'entrée
│   ├── menu.py        # Interface terminal
│   ├── api.py         # Connexion API Brickset
│   ├── config.py      # Configuration
│   └── generator.py   # Génération HTML
├── assets/
│   ├── css/           # Styles
│   ├── js/            # Scripts
│   ├── images/        # Ressources images
│   └── templates/     # Templates HTML
├── DATA/              # Fichiers générés
├── requirements.txt
└── .env.example
```

## Auteurs

- [Yanis STENTZEL](https://yanisstentzel.github.io/)
- [Jonathan WILD](https://www.linkedin.com/in/jonathan-wild-b7986434a/)
- [Alix CARTAL](https://www.linkedin.com/in/alix-cartal-18333534b/)

## Licence

Projet académique - IUT2 Grenoble - 2024-2025