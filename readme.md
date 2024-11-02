# Application de Chat Interactive pour PDF avec IA Conversationnelle

## Vue d'ensemble du projet

Ce projet vise à développer une application interactive permettant aux utilisateurs de consulter et d'interagir avec le contenu de documents PDF en utilisant le langage naturel. L'application intègre diverses techniques de traitement du langage naturel (NLP) et d'apprentissage automatique pour faciliter une récupération efficace et précise des informations à partir des PDF. Elle répond à un besoin courant des individus et des organisations : extraire rapidement et efficacement des informations pertinentes de grandes collections de documents.

Le cœur de l'application est alimenté par un modèle d'IA conversationnelle capable de comprendre et de répondre aux requêtes des utilisateurs en se basant sur le contenu des documents PDF téléchargés. Le système est conçu pour être convivial et accessible, avec une interface web développée avec Streamlit. L'objectif principal est d'améliorer l'efficacité de la récupération d'informations à partir des PDF, facilitant ainsi la recherche d'informations spécifiques sans avoir à parcourir manuellement des pages de texte.

![Interface Screenshot](screenshot.JPG)

## Fonctionnalités

- Téléchargement de PDF : Permet aux utilisateurs de télécharger plusieurs documents PDF.
- Extraction de texte : Extraction automatique du contenu textuel des PDF téléchargés.
- Recherche intelligente : Utilisation de techniques avancées de NLP pour répondre aux requêtes des utilisateurs.
- Validation des réponses : Vérification de la pertinence et de l'exactitude des réponses générées.
- Interface conviviale : Interface web interactive développée avec Streamlit pour une expérience utilisateur optimale.
- Sauvegarde des réponses : Possibilité de sauvegarder les réponses générées comme notes pour une consultation ultérieure.

## Technologies Utilisées

- Langages de programmation : Python
- Bibliothèques NLP :
PyPDF2 pour l'extraction de texte des PDF.
LangChain pour le découpage récursif des textes.
Sentence Transformers pour la création d'embeddings de texte.
- Bases de données vectorielles :
FAISS pour le stockage et la recherche efficace des vecteurs de texte.
- Modèles de Langage :
LLaMA pour la génération de réponses.
- Frameworks Web :
Streamlit pour le développement de l'interface utilisateur.
- Gestion de versions :
Git et GitHub pour le contrôle de version et la collaboration.

## Utilisation

1. Clone the repository::

    ```bash
    git clone https://github.com/your-repo/interactive-pdf-chat.git
    cd interactive-pdf-chat
    ```

2. Create and activate a virtual environment::

    ```bash
    python3 -m venv env
    source env/bin/activate  # On Windows: env\Scripts\activate

    ```


3. Install dependencies:

    ```bash
    pip install -r requirements.txt

    ```

4. Run the application:
    ```bash
   streamlit run app.py

    ```
5. Open the app in your browser: http://localhost:8501
   
## Project Structure

- .env: Variables d'environnement pour configurer l’application.
- htmlTemplate.py: Modèle HTML pour afficher les réponses.
- note.txt: Fichier de sauvegarde des réponses générées.
- readme.md: Instructions pour démarrer le projet.
- StreamlitApp.py: Fichier principal de l'interface Streamlit.
- vectorstore: Dossier pour la base de données de vecteurs (FAISS).
- pycache: Cache Python pour accélérer l'exécution.

## References

- FAISS Documentation: https://faiss.ai/
- LLaMA Language Model: https://ai.facebook.com/blog/large-language-model-llama-meta-ai/
- Streamlit Documentation: https://docs.streamlit.io/



