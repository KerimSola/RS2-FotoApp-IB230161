# FotoApp

**Platforma za rezervaciju termina za fotografisanje i pregled fotografa**

Seminarski rad iz predmeta **Razvoj softvera 2**
Univerzitet „Džemal Bijedić" Mostar, Fakultet informacijskih tehnologija

- **Student:** Kerim Solić (IB230161)
- **Profesori:** Prof. dr Denis Mušić, Doc. dr Elmir Babović

## Opis

FotoApp povezuje klijente koji traže fotografske usluge sa profesionalnim fotografima. Omogućava pretragu fotografa i portfolija, uvid u slobodne termine, online rezervaciju i plaćanje.

- **Mobilna aplikacija** (klijenti): pretraga fotografa po kategorijama, gradu, cijeni i ocjeni, pregled portfolija, rezervacija termina, Stripe plaćanje, recenzije, favoriti, notifikacije i preporuke.
- **Desktop aplikacija** (fotografi/administratori): upravljanje profilom, portfolijom, cjenovnikom i paketima, kalendarom dostupnosti i rezervacijama, statistika i PDF izvještaji.

## Tehnologije

- ASP.NET Core (.NET 8) REST API – `FotoApp.API`
- Pomoćni servis – `FotoApp.Worker` (RabbitMQ: email potvrde, QR kodovi, podsjetnici)
- SQL Server (baza `IB230161`), Entity Framework Core
- RabbitMQ, Docker / docker-compose
- Stripe (sandbox), JWT autentifikacija

## Pokretanje

1. Kopirati `.env.example` u `.env` i upisati vrijednosti.
2. Pokrenuti `docker compose up --build`.

## Status

🚧 Projekat je u razvoju.
