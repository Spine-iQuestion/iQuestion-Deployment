# Opzetten iQuestion

Deze repository leent zich voor het uitrollen van de iQuestion applicatie.

## Benodigdheden

* [Git](https://git-scm.com/downloads)
* [Docker](https://docs.docker.com/get-docker/)
* [Docker Compose](https://docs.docker.com/compose/install/)

Windows gebruikers kunnen [Docker Desktop](https://docs.docker.com/desktop/install/windows-install/) downloaden, daar zit Docker Compose al ingebouwd.

## Hoe te gebruiken?

0. *Controleer altijd een script voor je deze uitvoert in de terminal!*
1. Open  een **nieuwe** terminal (nadat je de benodigdheden hebt geïnstalleerd)
2. Browse naar een folder waarin je de applicatie wilt zetten en clone deze repository:

```Bash
git clone https://github.com/IPSEN2/iQuestion-Deployment
```

3. Navigeer naar de nieuwe folder

```Bash
cd iQuestion-Deployment
```

3. Kopieëer het bestand `.env.example` naar een nieuw bestand genaamd `.env` en vul het bestand in met je omgevingsvariablen

4. Pas de hostnaam aan in dit bestand:

`iQuestion-Angular\src\environments\environment.prod.ts`

5. Daarna kan je de applicatie deployen

```Bash
# Voor Windows
./deploy_windows.bat
```

```Bash
# Voor Linux en MacOS
chmod +x ./deploy_linux.sh
sudo ./deploy_linux.sh
```
