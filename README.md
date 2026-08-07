# Twoje Discord bio — instrukcja uruchomienia

## 1. Wrzuć pliki na GitHub

1. Wejdź na github.com i utwórz nowe **publiczne** repozytorium, np. `discord-bio`.
2. Wgraj do niego 4 pliki z tego folderu: `index.html`, `admin.html`, `profile.json`, oraz pusty folder `assets` (możesz dodać do niego plik `.gitkeep`, żeby Git go zachował).
   - Najprościej: przeciągnij pliki na stronę repo w przeglądarce (przycisk "Add file" → "Upload files").

## 2. Włącz GitHub Pages

1. W repo wejdź w **Settings → Pages**.
2. Przy "Source" wybierz branch `main`, folder `/ (root)`.
3. Zapisz. Po chwili Twoja strona będzie dostępna pod:
   `https://twojnick.github.io/discord-bio/`

To jest link, który wklejasz w bio Discorda.

## 3. Wygeneruj token GitHub (żeby panel admina mógł zapisywać zmiany)

1. Wejdź na: https://github.com/settings/tokens/new
2. W "Note" wpisz np. `discord-bio-admin`.
3. Zaznacz uprawnienie **repo** (cały checkbox z tej sekcji).
4. Kliknij "Generate token" na dole.
5. **Skopiuj token od razu** (zaczyna się od `ghp_...`) — GitHub pokaże go tylko raz.

⚠️ Token działa jak hasło do Twojego konta w zakresie repozytoriów. Nie wrzucaj go nigdzie publicznie. Panel admina trzyma go tylko lokalnie w Twojej przeglądarce (localStorage), nigdzie go nie wysyła poza GitHub.

## 4. Edytuj swój profil

1. Otwórz `https://twojnick.github.io/discord-bio/admin.html`
2. Wklej token i nazwę repo (`twojnick/discord-bio`) → "Połącz i wczytaj profil".
3. Zmieniaj kolory, tekst, zdjęcia — po prawej widzisz podgląd na żywo.
4. Kliknij **"Zapisz i opublikuj"**. Strona zaktualizuje się w ~30-60 sekund.

## 5. (Opcjonalnie) Discord Presence — status na żywo

1. Dołącz na serwer Discord **Lanyard**: https://discord.gg/lanyard (samo dołączenie włącza tracking Twojego statusu).
2. Skopiuj swoje Discord ID (Ustawienia Discord → Zaawansowane → włącz Tryb dewelopera, potem PPM na swój profil → "Kopiuj ID użytkownika").
3. Wklej to ID w panelu admina w polu "Discord ID".

## Uwaga o bezpieczeństwie panelu admina

`admin.html` jest technicznie dostępny pod publicznym linkiem — ale **bez Twojego tokena nikt nic nie zapisze** do Twojego repo (token trzeba wkleić ręcznie, a Ty jesteś jedyną osobą, która go ma). Jeśli chcesz dodatkowo ukryć sam link do panelu, po prostu nikomu go nie wysyłaj — nie ma potrzeby robić nic więcej.
