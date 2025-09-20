# ZoneCode-API

ZoneCode-API to lekki i wszechstronny plugin dla serwerów Minecraft opartych na Paper/Spigot, który jest **wymagany** do działania wszystkich innych pluginów spod szyldu ZoneCode. Zapewnia podstawowe funkcje zarządzania serwerem, takie jak wyświetlanie informacji o serwerze, przeładowanie konfiguracji oraz sprawdzanie aktualizacji. Plugin integruje się również z bStats w celu zbierania anonimowych statystyk użytkowania.

## Funkcje

- **Komenda informacyjna**: Użyj `/zonecode`, aby wyświetlić informacje o serwerze z brandingiem ZoneCode, w tym dane o autorach, stronie internetowej i serwerze Discord.
- **Komenda pomocy**: Uruchom `/zonecode help`, aby zobaczyć listę dostępnych komend, dostosowaną do uprawnień użytkownika.
- **Przeładowanie pluginu**: Przeładuj konfigurację pluginu za pomocą `/zonecode reload` bez konieczności restartowania serwera.
- **Automatyczne aktualizacje**: Sprawdź i zainstaluj najnowszą wersję pluginu za pomocą `/zonecode update` (wymaga skonfigurowanego adresu URL aktualizacji).
- **Konfigurowalne komunikaty**: Dostosuj prefiksy komunikatów i inne ustawienia w pliku `config.yml`.
- **Wsparcie dla uprawnień**: Precyzyjne uprawnienia do kontroli dostępu do komend (`zonecode.use`, `zonecode.reload`, `zonecode.update`).

## Wymagania

- **Serwer Minecraft**: Paper lub Spigot (KAŻDA WERSJA).
- **Java**: Wersja 8 lub wyższa.

## Instalacja

1. **Pobierz plugin**:
   - Pobierz najnowszy plik `ZoneCode-API.jar` ze strony Releases.
2. **Umieść w folderze pluginów**:
   - Skopiuj plik JAR do folderu `plugins/` na serwerze.
3. **Uruchom/Przeładuj serwer**:
   - Uruchom serwer Paper/Spigot, aby wygenerować plik `plugins/ZoneCode-API/config.yml`.
4. **Konfiguracja (opcjonalna)**:
   - Edytuj plik `config.yml`, aby dostosować prefiks komunikatów lub inne ustawienia.

## Komendy

| Komenda | Opis | Uprawnienie |
| --- | --- | --- |
| `/zonecode` | Wyświetla informacje o serwerze od ZoneCode. | `zonecode.use` |
| `/zonecode help` | Pokazuje listę dostępnych komend. | `zonecode.use` |
| `/zonecode reload` | Przeładowuje konfigurację pluginu. | `zonecode.reload` |
| `/zonecode update` | Sprawdza i instaluje aktualizacje pluginu. | `zonecode.update` |

**Aliasy**: `/developer`, `/dev`, `/development`

## Uprawnienia

- `zonecode.use` (domyślnie: true): Pozwala na użycie komend `/zonecode` i `/zonecode help`.
- `zonecode.reload` (domyślnie: op): Pozwala na użycie komendy `/zonecode reload`.
- `zonecode.update` (domyślnie: op): Pozwala na użycie komendy `/zonecode update`.

## Konfiguracja

Plugin generuje plik `config.yml` w folderze `plugins/ZoneCode-API/` z następującymi domyślnymi ustawieniami:

```yaml
# Konfiguracja ZoneCode-API
version: 1.0
message-prefix: "§5[ZoneCode] §r"
```

Możesz zmodyfikować `message-prefix`, aby dostosować prefiks komunikatów wyświetlanych przez plugin.

## Budowanie ze źródeł

1. Sklonuj repozytorium:

   ```bash
   git clone https://github.com/ZoneCode-Team/ZoneCode-API.git
   ```

2. Skompiluj plugin za pomocą Mavena:

   ```bash
   mvn clean package
   ```

3. Znajdź skompilowany plik `ZoneCode-API.jar` w folderze `target/`.

## Wkład w rozwój

Zachęcamy do współpracy! Prześlij pull requesty lub zgłaszaj problemy na repozytorium GitHub.

1. Sforkuj repozytorium.
2. Stwórz nową gałąź (`git checkout -b feature/twoja-funkcja`).
3. Zatwierdź zmiany (`git commit -m 'Dodaj swoją funkcję'`).
4. Wypchnij gałąź (`git push origin feature/twoja-funkcja`).
5. Otwórz pull request.

## Wsparcie

- **Strona internetowa**: zonecode.dev
- **Discord**: dc.zonecode.dev
- **Problemy**: Zgłaszaj błędy lub sugestie na stronie Issues.

## Licencja

Projekt jest licencjonowany na licencji MIT. Zobacz plik LICENSE dla szczegółów.

## Podziękowania

Stworzone przez ZoneCode Team. Dziękujemy za korzystanie z ZoneCode-API! Ten plugin jest wymagany do działania wszystkich innych pluginów od ZoneCode.
