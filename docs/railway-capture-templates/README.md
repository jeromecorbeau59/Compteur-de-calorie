# Modèle de captures d'écran pour le déploiement Railway

Ce dossier contient des modèles de captures d'écran (placeholders) et un guide pour les captures demandées lors du déploiement sur Railway.

Fichiers attendus (noms et légendes) :

- capture_00_backend_local_health.png — Résultat de `curl http://localhost:8001/api/health` montrant `{"status":"healthy"}`
- capture_01_frontend_build.png — Arborescence du dossier `frontend` après `yarn build` (montrer le dossier `build`)
- capture_02_select_repo.png — Sélection du repo dans Railway (écran "Deploy from GitHub")
- capture_03_backend_service_setup.png — Configuration du service backend (Docker or Python) dans Railway
- capture_04_add_mongodb.png — Ajout du plugin MongoDB dans Railway (affichage de `MONGO_URL`)
- capture_05_backend_env_vars.png — Variables d'environnement backend (MONGO_URL, JWT_SECRET...)
- capture_06_backend_deployed.png — Page du service backend montrant l'URL publique
- capture_07_backend_health_prod.png — Réponse de l'endpoint `/api/health` en production
- capture_08_frontend_service_setup.png — Configuration du service Static Site pour frontend (root=frontend, build=yarn build, publish=build)
- capture_09_frontend_deployed.png — Frontend déployé : URL publique Railway
- capture_10_frontend_app_open.png — Page d'accueil de l'application frontend (affichage du site)
- capture_11_register_test.png — Capture de l'inscription utilisateur réussie (ou erreur affichée)

Conseils pour les captures :
- Résolution recommandée : 1280×720 ou 1920×1080.
- Recadrez pour n’afficher que la zone utile (logs, URL, ou la partie d'application).
- Nommez les fichiers exactement comme ci‑dessus et placez‑les dans ce dossier.
