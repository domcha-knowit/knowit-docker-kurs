---
marp: true
theme: default
style: |
    img[alt~="center"] {
      display: block;
      margin: 0 auto;
    }
---

# En grundläggande kurs i Linux, AWS och SSH

---

# Detta behövs inför kursen

Windows-datorer
1. Datorer med Windows behöver ha Putty installerad.
2. aws-linux-demo.ppk filen behöver sparas ned. Filen går att hitta på [Länk](https://knowit.sharepoint.com/:f:/r/sites/O365-Development/Shared%20Documents/Cloud%20native/SSH-key?csf=1&web=1&e=qbYYiW). Spara ned aws-linux-demo.ppk på valfri plats på hårddisken.

MacOS/Linux datorer
1. Datorer med MacOS och Linux har terminalprogram förinstallerad och behöver därför inte installera något särskilt program.
2. aws-linux-demo.pem filen behöver sparas ned. Filen går att hitta på [Länk](https://knowit.sharepoint.com/:f:/r/sites/O367-Development/Shared%20Documents/Cloud%20native/SSH-key?csf=1&web=1&e=qbYYiW). Spara ned awd-linux-demo.pem på ~/.ssh/ katalogen.

---

# Introduktion:


Mentimeter -
 
---

# Installera Docker på Ubuntu 22.04
Följande länk på DigitalOcean visar hur Docker Engine installeras på Ubuntu [Länk](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-22-04).

`sudo apt install docker-ce`

---

# Övningar:
1. Starta en nginx container.
2. Stoppa nginx containern som du startade i steg 1.
3. Rensa alla stoppade container med system prune kommandot.
4. Skapa en index.html fil med grundläggande HTML kod med texten "Hej från Docker!". Starta en nginx container som monterar index.html på /usr/share/nginx/html.
5. Ladda ned dockerimagen kanboard/kanboard. (https://hub.docker.com/r/kanboard/kanboard/). Deploya den lokalt med hjälp av Docker och försök att navigera till applikationen.

---

# Frågor:
1. 
2. 
3. 
4. 

---

# Avslut och utvärdering:

Mentimeter - 

---
