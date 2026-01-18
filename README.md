# DayZ Offline / Single Player Launcher 🧟‍♂️

Jednoduchý `.bat` skript pro spuštění **lokálního offline serveru** pro hru DayZ. Tento skript ti umožní hrát DayZ v režimu "Single Player" (LAN), testovat nové updaty, stavět základny nebo prostě hrát bez ostatních hráčů

---

## 🚀 Jak tento skript použít

### 1. Příprava
Ujisti se, že máš ve Steamu nainstalovaný nástroj **DayZ Server**.
*(Najdeš v Knihovna -> Nástroje -> DayZ Server)*

### 2. Vytvoření souboru
1. Zkopíruj kód ze souboru v tomto repozitáři.
2. Otevři **Poznámkový blok** (Notepad).
3. Vlož kód.
4. Klikni na `Soubor` -> `Uložit jako`.
5. **Důležité:** U položky "Uložit jako typ" vyber **Všechny soubory (*.*)**.
6. Soubor pojmenuj `start.bat`.
7. Ulož tento soubor přímo do složky, kde máš nainstalovaný DayZ Server (např. `...\steamapps\common\DayZServer`).

### 3. Úprava cest (DŮLEŽITÉ ⚠️)
Pokud máš DayZ nainstalované na jiném disku než `C:`, nebo v jiné složce, musíš v kódu upravit cestu!

V řádku, který začíná `cd "C:\Program Files (x86)..."`, přepiš cestu tak, aby odpovídala tvému umístění složky **DayZServer**.

---

## 🗺️ Jak změnit mapu (Chernarus / Livonia / Sakhal)

Mapu změníš v souboru `serverdz.cfg` (najdeš ho ve složce DayZServer).
Hledej řádek `template="dayzoffline.chernarusplus";` na konci souboru.

Přepiš ho podle toho, jakou mapu chceš hrát:

*   **Chernarus:** `dayzoffline.chernarusplus`
*   **Livonia:** `dayzoffline.enoch`
*   **Sakhal (Frostline):** `dayzoffline.sakhal`

---

## 💾 Ukládání postavy a WIPE

*   Server automaticky ukládá postup při korektním vypnutí.
*   Postup (savy) najdeš ve složce: `mpmissions\dayzoffline.[název_mapy]\storage_1\`
*   Pokud chceš začít od začátku (**WIPE**), stačí smazat celou složku `storage_1`.

---

## ⚠️ Řešení problémů
*   Pokud se okno konzole po spuštění hned zavře, pravděpodobně máš špatně nastavenou cestu k souborům v `.bat` souboru.
*   Počkej, dokud v konzoli neuvidíš hlášku, že inicializace proběhla úspěšně. Teprve poté zapni hru DayZ, jdi do **LAUNCHER** -> **LAN** a připoj se.

---

*Tento skript slouží pro vytvoření základního Vanilla serveru pro osobní použití.*
