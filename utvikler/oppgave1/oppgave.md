# Oppgave

Lag en enkel applikasjon som kjører i et Kubernetes cluster med tilhørende dockerfile og Kubernetes manifester. Applikasjonen skal kunne deployes i et Kubernetes cluster ved bruk av `kubectl apply -f prosjekt/`. Husk at URL til konteinerbildet må være tilgjengelig for oss når vi skal teste. Bruk gjerne ghcr.io eller Docker Hub. 

Applikasjonen skal på endepunktet `/origo` returnere en oversikt over alle stasjoner fra endepunkt beskrevet under. Dette trenger bare returneres som rådata.

Tips: Du kan bruke for eksempel k3d, minikube eller k3s for å bygge og teste Kubernetes manifestene dine om du ikke har et cluster tilgjengelig.

Krav
* Applikasjon skal lages som en docker-container som skal kunne returnere stasjoner fra oslo-bysykkel api
  ** Dokumentasjon: https://oslobysykkel.no/apne-data/sanntid
  ** Endepunkt: https://gbfs.urbansharing.com/oslobysykkel.no/station_information.json
* URL til bysykkel-API-endepunktet må komme inn gjennom miljøvariabel
* Så lang det lar se gjøre: følge best practices for Dockerfile og Kubernetes manifester
* Bruk et valgfritt programmeringsspråk
* Docker image skal lastes opp på docker hub eller liknende (slik at kan kjøres av oss)
* Koden levers som et åpent github repository
