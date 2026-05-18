# 📊 News Data Platform - Architecture Medallion

Une plateforme de traitement et d'ingénierie de données d'actualités en temps réel, construite selon l'Architecture Medallion (Bronze, Silver, Gold). Le projet intègre un pipeline ETL complet, une automatisation et un dashboard de monitoring haut de gamme avec un système de gouvernance des données sécurisé.

---

## 👥 Équipe de Développement
* **Marwa El Omari Alaoui**
* **Chaimaa Ezzerag**
* **Sasam (Mr Fruit)**

---

## ✨ Points Clés du Projet
* **Pipeline ETL Fiable :** Ingestion, nettoyage et agrégation automatique des flux d'actualités.
* **Architecture Medallion :** Structuration rigoureuse des tables sous PostgreSQL en trois niveaux (Données brutes ➡️ Nettoyées ➡️ Agrégées pour le business).
* **Infrastructure Containerisée :** Déploiement et gestion de la base de données via Docker et Docker Compose pour une portabilité totale.
* **Dashboard Premium "From Scratch" :** Développement d'une interface de monitoring ("Executive Slim") sous Streamlit. Aucun template tout fait n'a été utilisé : le design complet a été codé manuellement en HTML5 et CSS3 pour garantir un rendu sobre et professionnel.
* **Gouvernance des Données :** Module de sécurité avec authentification. Les utilisateurs invités ont accès aux graphiques en lecture seule, tandis que l'accès Admin active les fonctionnalités CRUD pour interagir et modifier la base PostgreSQL directement depuis l'interface.

---

## 🏗️ Technologies Utilisées
* **Langage principal :** Python 3.10+
* **Base de données :** PostgreSQL
* **Conteneurisation :** Docker / Docker Compose
* **Visualisation & UI :** Streamlit, Plotly, HTML5, CSS3
* **Connecteur Database :** Psycopg2

---

## 📁 Structure du Dépôt
```plaintext
news-data-platform/
├── app.py                  # Dashboard Streamlit avec injection HTML/CSS Custom
├── data/
│   └── scripts/            # Scripts Python pour le pipeline ETL (Bronze -> Silver -> Gold)
├── docker-compose.yml      # Configuration du conteneur PostgreSQL
└── README.md               # Documentation technique du projet
