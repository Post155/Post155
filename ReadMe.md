# Mein Projekt

Eine kurze Beschreibung des Projekts.

## Features

- Benutzeranmeldung
- Chat-Funktion
- Datenbankanbindung
- Responsive UI

## Voraussetzungen

- Git
- Python 3.12
- VS Code

## Installation

```bash
git clone https://github.com/benutzer/mein-projekt.git
cd mein-projekt
pip install -r requirements.txt
```

## Verwendung

```bash
python main.py
```

## Projektstruktur

```text
mein-projekt/
├── src/
│   ├── main.py
│   ├── database.py
│   └── ui.py
├── tests/
├── docs/
├── requirements.txt
└── README.md
```

## Git-Workflow

```mermaid
gitGraph
    commit id: "Projekt erstellt"

    branch develop
    checkout develop
    commit id: "Projektstruktur"

    branch feature-login
    checkout feature-login
    commit id: "Login UI"
    commit id: "Login Logik"

    checkout develop
    merge feature-login

    branch feature-chat
    checkout feature-chat
    commit id: "Chat UI"
    commit id: "Nachrichten senden"

    checkout develop
    merge feature-chat

    checkout main
    merge develop
    commit id: "Release v1.0"

    branch hotfix
    checkout hotfix
    commit id: "Fehlerbehebung"

    checkout main
    merge hotfix
    commit id: "Release v1.0.1"
```

## Entwicklungsablauf

1. Feature-Branch erstellen
2. Änderungen entwickeln
3. Pull Request öffnen
4. Review durchführen
5. Merge in `develop`
6. Release nach `main`

## Screenshots

docs/login.png

## Lizenz

MIT License

## Autor

Jonas Schröder