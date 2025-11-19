Mon Projet Netmiko
# === PARTIE I ===
mkdir prenom-nom-netmiko
cd prenom-nom-netmiko
git init

# === PARTIE II ===
echo "# Mon Projet Netmiko" > README.md
touch main.py
git add README.md
git commit -m "Ajout du fichier README.md"
echo 'print("Hello, Git!")' > main.py
git add main.py
git commit -m "Ajout du script Python principal"
git log --oneline

# === PARTIE III ===
git checkout -b feature/netmiko
# (modifier main.py avec la fonction acces_netmiko)
git add main.py
git commit -m "Ajout de la fonction acces_netmiko"
git checkout main
git merge feature/netmiko

# === PARTIE IV ===
git remote add origin https://github.com/username/prenom-nom-netmiko.git
git push -u origin main
# (créer feature/salut sur GitHub)
git fetch origin
git checkout feature/salut
# (modifier main.py avec la fonction dire_salut)
git add main.py
git commit -m "Ajout de la fonction dire_salut"
git push origin feature/salut
# (créer et accepter la Pull Request sur GitHub)
git checkout main
git pull origin main
<img width="531" height="134" alt="image" src="https://github.com/user-attachments/assets/7e380956-77c5-47dc-9c8c-1439b97f7305" />


       
