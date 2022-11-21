---
marp: true
theme: default
style: |
    img[alt~="center"] {
      display: block;
      margin: 0 auto;
    }
---

# En grundläggande kurs i Docker

```
 ____             _                
|  _ \  ___   ___| | _____ _ __  
| | | |/ _ \ / __| |/ / _ \ '__| 
| |_| | (_) | (__|   <  __/ |   
|____/ \___/ \___|_|\_\___|_|   

```
##### presenterad av Dominic Chan, dominic.chan@knowit.se

---

# Detta behövs inför kursen

Windows-datorer
1. Datorer med Windows behöver ha Putty installerad.
2. aws-linux-demo.ppk filen behöver sparas ned. Filen går att hitta på [Länk](https://knowit.sharepoint.com/:f:/r/sites/O365-Development/Shared%20Documents/Cloud%20native/SSH-key?csf=1&web=1&e=qbYYiW). Spara ned aws-linux-demo.ppk på valfri plats på hårddisken.

MacOS/Linux datorer
1. Datorer med MacOS och Linux har terminalprogram förinstallerad och behöver därför inte installera något särskilt program.
2. aws-linux-demo.pem filen behöver sparas ned. Filen går att hitta på [Länk](https://knowit.sharepoint.com/:f:/r/sites/O365-Development/Shared%20Documents/Cloud%20native/SSH-key?csf=1&web=1&e=qbYYiW). Spara ned awd-linux-demo.pem på ~/.ssh/ katalogen.

---

# Vad är Docker?

- Containrar är som snabba och lättviktiga virtuella maskiner.
- Docker gör det enkelt att bygga och köra våra applikationer i containrar.

 
---

# Bare metal
![h:400px center](./images/baremetal.png)


---

# Virtual Machines
![h:400px center](./images/VM_arch.png)


---

# Containers
![h:400px center](./images/containers.png)


---

# VMs vs. Containers
![h:400px left bottom](./images/VM_arch.png)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![h:250px right bottom](./images/containers.png)


---

# Installera Docker på Ubuntu 22.04
Följande länk på DigitalOcean visar hur Docker Engine installeras på Ubuntu [Länk](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-22-04).

`sudo apt install docker-ce`

---

# Bygg en Docker containerimage från Dockerfile

Kör kommandot `docker build -t docker-demo-app .`

Docker kommer att per default att leta efter Dockerfile. Om du vill specificera filen kör då kommandot `docker build -f Dockerfile -t docker-demo-app .`

---

# Kör igång Docker container

Använd kommandot `docker run -d -p 8080:80 docker-demo-app`

---

# Visa alla containrar som körs

Använd kommandot `docker ps -a`

---

# Gör ett testanrop till docker-demo-app containern

Använd kommandot `curl localhost:8080`

---

# Stoppa docker-demo-app containern

Använd kommandot `docker stop <container-id>`

---

# Rensa alla stoppade containrar

Använd kommandot `docker system prune` och svara `ja` för att bekräfta

---

# Ladda ned container image från Dockerhub

Använd kommandot `docker pull busybox`

---

# Visa alla container images som finns sparat lokalt

Använd kommandot `docker images`

---

# Ta bort container image som finns sparat lokalt

Använd kommandot `docker rmi <imageid>`

---

# Övningar:
1. Starta container imagen bkimminich/juice-shop som lyssnar på port 3000.
2. Testa att containern bkimminich/juice-shop körs.
3. Stoppa containern som du startade i steg 1.

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
