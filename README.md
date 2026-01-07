# 🌦 Aplikacja pogodowa (Weather App)

Nowoczesna aplikacja pogodowa typu **frontend**, zbudowana w czystym **HTML, CSS i JavaScript**, korzystająca z **zewnętrznych API pogodowych** oraz map.

Projekt został stworzony jako **realistyczne ćwiczenie developerskie**, z naciskiem na:
- pracę z API,
- obsługę lokalizacji,
- debugowanie prawdziwych problemów produkcyjnych.

---

## 🚀 Funkcjonalności

- 🔍 **Wyszukiwanie miast (autocomplete)**
  - dynamiczne podpowiedzi miast (OpenStreetMap / Nominatim)
  - brak błędnych lokalizacji

- 📍 **Moja lokalizacja**
  - wykorzystanie `Geolocation API`
  - obsługa ograniczeń lokalizacji na desktopie (IP-based)
  - poprawne rozróżnienie: lokalizacja przybliżona vs dokładna (mobile)

- 🗺️ **Mapa**
  - Leaflet + OpenStreetMap
  - marker aktualnej lokalizacji

- 🌡️ **Aktualna pogoda**
  - dane z API **meteoblue**

- 📅 **Prognoza 7-dniowa**
  - temperatury minimalne i maksymalne

- 📊 **Wykres temperatur**
  - Chart.js
  - czytelna wizualizacja trendu temperatur

---

## 🧠 Ważne informacje (ograniczenia techniczne)

### Lokalizacja na desktopie
Na komputerach stacjonarnych (np. **Windows 11 + Chrome/Edge**):
- przeglądarka **nie posiada prawdziwego GPS**,
- lokalizacja jest często określana na podstawie **adresu IP**,
- dokładność może wynosić nawet **kilkaset kilometrów** (np. miasto regionalne).

👉 Jest to **ograniczenie środowiska**, a nie błąd aplikacji.

### Lokalizacja na urządzeniach mobilnych
Na smartfonach:
- wykorzystywany jest fizyczny GPS,
- dokładność: **5–20 metrów**,
- aplikacja poprawnie wskazuje faktyczną miejscowość.

---

## 🛠️ Technologie

- **HTML5**
- **CSS3**
- **JavaScript (ES6+)**
- **meteoblue API** – dane pogodowe
- **OpenStreetMap / Nominatim** – geokodowanie i autocomplete
- **Leaflet.js** – mapa
- **Chart.js** – wykresy

---

## ⚙️ Uruchomienie projektu

1. Sklonuj repozytorium:
```bash
git clone https://github.com/twoj-login/weather-app.git
```

2. Otwórz plik `index.html`:
- najlepiej przez **Live Server (VS Code)**
- lub przez `http://localhost`

3. W pliku `index.html` wstaw swój klucz API:
```js
const METEOBLUE_KEY = "TWOJ_KLUCZ_API";
```

---

## 📌 Czego nauczył mnie ten projekt

- pracy z zewnętrznymi API
- obsługi `async / await`
- debugowania błędów JavaScript
- rozumienia działania lokalizacji w przeglądarce
- różnic między desktopem a mobile
- podejmowania decyzji projektowych (kiedy **nie dodawać** kolejnych funkcji)

---

## 📄 Licencja

Projekt edukacyjny – do dowolnego wykorzystania w celach nauki i portfolio.
