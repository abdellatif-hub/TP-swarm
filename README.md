# 🚀 TP Docker Swarm – Déploiement d'une Application Flask

Ce projet montre comment déployer une application **Flask** dans un cluster **Docker Swarm**, avec :
- 📌 3 réplicas
- 🔐 Docker Secrets
- ⚙️ Load Balancing
- 📦 Stack complète (stack.yml)

---

## 📁 Arborescence du TP
````
docker_tp12/
├── app/
│ ├── app.py
│ ├── requirements.txt
│ └── Dockerfile
├── secret.txt
└── stack.yml
````
<img width="708" height="948" alt="image" src="https://github.com/user-attachments/assets/a3add8a3-430c-45f7-8d13-b1746454c7d8" />

---

## 🔐 2. Création du Secret
````
docker secret create app_secret secret.txt
````
<img width="1631" height="112" alt="image" src="https://github.com/user-attachments/assets/1c7f3e9e-83a4-4628-8268-d4030aa8b96a" />

---
## 📦 3. Déploiement de la Stack
````
Commande :

docker stack deploy -c stack.yml tp12
````
<img width="1604" height="214" alt="image" src="https://github.com/user-attachments/assets/8803fe0b-89c8-40a4-809d-392167ab78a4" />

---
## 📊 4. Vérification des Services
````
docker service ls
````
<img width="1594" height="148" alt="image" src="https://github.com/user-attachments/assets/52df8d59-1e97-4a67-bba9-e825af6b8723" />

---
## 🌐 6. Test dans le Navigateur
````
Ouvrir :

👉 http://localhost:8080
````

<img width="2559" height="1227" alt="image" src="https://github.com/user-attachments/assets/ff41ce17-09d7-439d-bcbc-8123b80eb9e4" />
<img width="2016" height="1178" alt="image" src="https://github.com/user-attachments/assets/67319467-4e63-4094-80bd-4f92ffb5aca6" />



