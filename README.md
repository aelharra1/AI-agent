# AI-agent

# Projet LLM Engineering - Agents Web et CSV

Développement d'agents intelligents pour l'extraction d'informations web et l'analyse de données CSV utilisant smolagents et langchain.

## Description

Ce projet développe deux types d'agents autonomes :
- **Agent Web** : Extraction d'informations dynamiques à partir de sites web
- **Agent CSV** : Recherche et exploitation rapide d'informations dans des fichiers CSV

L'objectif est de permettre une extraction facile et automatisée d'informations à partir de différentes sources de données.

## Architecture et Méthodologie

### Agent Web - Approche 1
```
MANAGER AGENT
├── Web Agent
│   ├── Extract Link Tool
│   └── Extract Content Tool
└── Image Agent
    └── Image Generator Tool
```

### Agent Web - Approche 2
```
Web Agent 2
├── Close Pop-up Tool
├── Go Back Tool
├── Get Current URL Tool
├── Search Item with Context Tool
└── Save Screenshot 
```

- Gestion de la navigation avec Helium/Selenium
- Firefox + GeckoDriver

### Agent CSV
```
CSV Agent
├── JSON RAG
│   ├── BM25
│   └── Hybride
└── LangChain
```

## Technologies Utilisées

- **smolagents** : Framework pour la création d'agents web
- **langchain** : Framework pour l'agent CSV et RAG
- **Selenium/Helium** : Automatisation de navigation web
- **Firefox + GeckoDriver** : Navigateur pour l'automatisation
- **BM25** : Algorithme de recherche et indexation

## Résultats et Performances

### Réussites
| Agent | Performance |
|-------|-------------|
| **Web Agent 1** | Réponses justes à des questions précises vérifiables en naviguant sur le site |
| **CSV Agent** | Réponses justes à des questions précises nécessitant la recherche dans plusieurs fichiers |

### Échecs et Limitations
| Agent | Problèmes Identifiés |
|-------|---------------------|
| **Web Agent 2** | Captures d'écran non prises en compte pour la navigation et l'extraction d'informations |
| **JSON RAG** | Mauvais contexte retrieved et mauvaises réponses à des questions simples |

## Auteurs

- **Abdelali El Harrani**
- **Abdoulaye Syll**

*Mastère VALDOM 2025*

---

Ce projet démontre le potentiel des agents LLM pour l'automatisation de l'extraction d'informations, avec des résultats prometteurs malgré les défis techniques rencontrés.
