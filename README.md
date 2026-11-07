# IA générative et RAG

Projet d'apprentissage autour de l'ingestion de documents, de la recherche vectorielle et de la création de pipelines RAG avec Python et LangChain.

## Contenu

- Notebooks d'ingestion de fichiers texte, PDF, Word, CSV, Excel et JSON
- Préparation et découpage des documents en chunks
- Création d'embeddings et indexation avec FAISS ou ChromaDB
- Recherche sémantique et pipelines RAG avec LangChain et LCEL
- Expérimentations autour de BM25, du classement et de l'évaluation des chunks

Les fichiers PDF, Word, Excel, les bases vectorielles et les fichiers de données locaux ne sont pas versionnés. Ajoutez vos propres documents dans le dossier `data` si vous souhaitez relancer les notebooks correspondants.

## Technologies

Python 3.12, LangChain, LCEL, OpenAI API, Sentence Transformers, FAISS, ChromaDB, PyMuPDF, pypdf, Unstructured, Jupyter.

## Installation

Avec [uv](https://docs.astral.sh/uv/) :

```bash
uv sync
```

Ou avec pip :

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

Sous Windows PowerShell, activez l'environnement avec :

```powershell
.venv\Scripts\Activate.ps1
```

## Configuration

Certains notebooks utilisent l'API OpenAI. Créez un fichier `.env` à la racine du projet et ajoutez votre clé :

```env
OPENAI_API_KEY=votre_cle_api
```

Le fichier `.env` est ignoré par Git. Ne publiez jamais de clé API dans un notebook ou dans le dépôt.

## Démarrage

Ouvrez le dossier dans Jupyter ou VS Code, puis lancez les notebooks dans `notebooks/`. Plusieurs exercices sont indépendants ; certains nécessitent un fichier source correspondant dans `data/` et une clé API valide.

## Données

Les exemples texte, CSV et JSON présents dans `data/` servent aux exercices. Vérifiez les droits et retirez toute donnée personnelle ou confidentielle avant d'ajouter un nouveau fichier.
