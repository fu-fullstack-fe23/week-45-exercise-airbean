# Airbean

Du ska bygga en webbapp där det går att beställa kaffe och få den levererad via drönare (drönare ingår ej i uppgiften). Självklart ska detta göras med Typescript för extra typsäkerhet!

Du bör inte a några `any` som datatyp i några av dina komponenter.

## Funktionalitet

* Gå att lägga till produkter i en varukorg (varukorgen ligger i din Zustand store)
* Hämta alla produkter med `fetch`, (du får köra axios om du vill)
* Kunna skicka sin order med `fetch` och alla produkter och få ett svar med en ETA och ordernummer
* När en beställning är lagd så töms ens zustand store
* Ifall man lagt en order och går till vyn för att se sin beställning ska ett anrop göras till API:et för att få tillbaka hur många minuter det är kvar. Om beställningen är leverad ska "Ingen aktiv beställning finns" visas.

## Level ups (ifall ni har tid över)

* Kunna lägga till flera av samma produkt i varukorgen
* Ta bort en produkt

## Figmaskiss
https://www.figma.com/file/Zpx8KqhL7g66JZ6MOhbxJ6/AirBean-v.1.1---Without-profile?node-id=0%3A1&t=4CJ1Zk2F2OnHOWJp-1

## API-dokumentation
https://airbean-9pcyw.ondigitalocean.app/api/docs/

**BASE URL**
```
https://airbean-9pcyw.ondigitalocean.app
```

Ni behöver enbart bry er om följande tre endpoints:

* /api/beans/
* /api/beans/order
* /api/beans/order/status/{orderNr}

## Bibliotek

Du kommmer behöva använda React router och Zustand till denna uppgift.

**Installationsinstruktioner**

`npm install react-router-dom`

`npm install zustand`
