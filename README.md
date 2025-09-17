# Guide de Lancement du Prototype IA –

## Prérequis

- Python 3.9+
- React
- npm
- FastAPI
- Uvicorn
- Vite
- Clé API OpenAI (ou Google Gemini)

## Lancement du Backend (FastAPI)

1. Créer un environnement virtuel :

   ```bash
   python -m venv venv
   # Sous Windows :
   venv\Scripts\activate
   ```

2. Installer les dépendances :

   ```bash
   pip install -r requirements.txt
   ```

3. Créer un fichier `.env` avec :

    ```env
    API_KEY=<ta_cle_api>
    ```

4. Lancer le serveur :

    ```bash
    uvicorn main:app --reload
    ```

5. Accès Swagger : <http://localhost:8000/docs>

## Lancement du Frontend (React + Vite)

1. Aller dans le dossier :

    ```bash
    cd frontend
    ```

2. Installer les dépendances :

    ```bash
    npm install
    ```

3. Lancer le projet :

    ```bash
    npm run dev
    ```

4. Interface : <http://localhost:5173>

### Optionnel : Dockerisation

1. Créer un Dockerfile pour backend et frontend

2. Créer un `docker-compose.yml`

3. Lancer avec :

    ```bash
    docker-compose up --build
    ```

## Vérification finale

- Swagger est accessible
- L’interface s’ouvre bien en local
- Les prompts sont envoyés à l’API
- Les cas de test sont générés

Accès à la BDD :  <https://cloud.mongodb.com/>
