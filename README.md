# TheWGMaximus
Sistema Zombie Realistico e Sincronizzato per QBCore
# 🧟 qb-zombies
**Fully Synced & Realistic Zombie System for QBCore**  
Version: `2.0.0`  
Author: **Max Lombardi**

---

## 📌 Description

`qb-zombies` is an advanced FiveM zombie script for **QBCore** framework, providing a fully **synced**, **immersive**, and **survival-based** zombie experience.

This script is ideal for roleplay, hardcore, or apocalypse-themed servers.

---

## 🔥 Features

- 🔄 Fully synced zombies (across all clients)
- 🧠 Realistic zombie movement & animations
- 💥 Audio immersion (HTML/NUI based)
- 🧪 Configurable zombie loot system
- 🔐 SafeZone support (no spawn)
- 🚫 Full ambient control (no traffic, no random peds)
- ⚙️ Optimized and easy to configure

---

## ⚙️ Requirements

- [qb-core](https://github.com/qbcore-framework/qb-core)
- [qb-inventory](https://github.com/qbcore-framework/qb-inventory)

---

## 📥 Installation

1. Place the `qb-zombies` folder inside your `resources` directory.
2. Add this to your `server.cfg`:
   ```
   ensure qb-zombies
   ```

---

## ⚙️ Configuration

All parameters are editable via `config.lua`.  
You can adjust zombie spawn count, intervals, loot items, and SafeZones.

---

## 📁 Folder Structure

```
qb-zombies/
├── client/
├── server/
├── html/
├── images/
├── config.lua
├── fxmanifest.lua
├── README.md
```

---

## 👤 Credits

> Developed and maintained by **Max Lombardi**  
> GitHub: [MaxLombardi237](https://github.com/MaxLombardi237)

---

## 📜 License

This script is released under the MIT License (see `LICENSE.md`).


contact  https://www.tiktok.com/@max_lombardi237

https://www.twitch.tv/maxlombardi237

https://discord.gg/zCZKGRqWa6


# 🧟 qb-zombies
**Sistema Zombie Realistico e Sincronizzato per QBCore**  
Versione: `2.0.0`  
Autore: **Max Lombardi**

---

## 📌 Descrizione

`qb-zombies` è uno script avanzato per server **FiveM** basati su **QBCore**, progettato per offrire un'esperienza zombie post-apocalittica completamente **sincronizzata**, **immersiva** e **realistica**.  

Include animazioni, loot, suoni ambientali, SafeZone configurabili e comportamento zombie credibile. Ideale per server survival, hardcore o roleplay zombie.

---

## 🎮 Caratteristiche principali

- 🔄 **Sincronizzazione totale** degli zombie tra tutti i giocatori
- 🧠 **Comportamento zombie realistico**: camminata lenta, attacchi con animazioni e suoni
- 💥 **Suoni immersivi** via NUI (HTML/JS)
- 📦 **Loot dinamico** con oggetti e parti di zombie
- 🔒 **SafeZone configurabili**
- 🚫 **Disabilitazione completa di traffico, NPC e polizia**
- 🧼 **Sistema pulito e ottimizzato**, facile da configurare
- 🔁 Compatibile con blackout, radiazioni, eventi militari e script custom

---

## ⚙️ Requisiti

- [qb-core](https://github.com/qbcore-framework/qb-core)
- [qb-inventory](https://github.com/qbcore-framework/qb-inventory)
- FiveM server (lua54 attivo)

---

## 📥 Installazione

1. Copia la cartella `qb-zombies` nella directory `resources` del tuo server.

2. Aggiungi al tuo `server.cfg`:


3. Assicurati che **qb-core** e **qb-inventory** siano avviati **prima** di questo script.

---

## 🔧 Configurazione

Modifica `config.lua` per personalizzare spawn, loot, SafeZone, distanza, ecc.

```lua
Config.SpawnZombie = 5                 -- Numero zombie ogni ciclo
Config.SpawnInterval = 10000           -- Tempo tra spawn (ms)
Config.MinSpawnDistance = 80
Config.MaxSpawnDistance = 120
Config.SafeZoneCoords = {
 { Pos = vector3(446.04, -993.56, 27.0), Radius = 40.0 },
 { Pos = vector3(-418.93, 1163.2, 325.9), Radius = 100.0 }
}

Config.Items – oggetti loot generici

Config.ZombieParts – loot anatomico (es. zombie_brain)

Config.ZombieSounds – suoni NUI (.ogg da riprodurre in html/sounds/)

Config.AddItem – oggetto bonus occasionale (es. kit medico)

🔊 Suoni
I suoni zombie vengono gestiti tramite html/index.html + script.js.
I file .ogg vanno posizionati in html/sounds/ e devono corrispondere ai nomi dichiarati in Config.ZombieSounds.

📁 Struttura della cartella

qb-zombies/
├── client/
│   └── main.lua
├── server/
│   └── main.lua
├── config.lua
├── fxmanifest.lua
├── README.md
├── html/
│   ├── index.html
│   ├── script.js
│   └── sounds/
│       └── *.ogg
├── images/
│   └── gas_lamp.png
│   └── gas_canister.png

🧪 Come funziona

Solo un client master è responsabile dello spawn zombie.

Gli zombie si spawnano periodicamente intorno al giocatore.

Ogni zombie è sincronizzato con il server tramite netId.

Quando uno zombie muore, si può saccheggiare premendo [E].

Loot e attacchi sono gestiti in modo sincronizzato.

Le SafeZone impediscono spawn in zone protette.

🧑‍💻 Crediti
Script ideato, scritto e sviluppato da Max Lombardi
GitHub: MaxLombardi237
Versione attuale: 2.0.0

❌ È vietata la rivendita.

❌ È vietato rimuovere i crediti all'autore.

✅ È consentito l'uso su server privati o pubblici.

✅ È consentita la modifica locale per uso personale.

📜 Licenza


© 2025 Max Lombardi - Tutti i diritti riservati.

contattatemi in privato su https://www.tiktok.com/@max_lombardi237

https://www.twitch.tv/maxlombardi237

https://discord.gg/zCZKGRqWa6
