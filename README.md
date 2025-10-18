# ZoneCode-API

ZoneCode-API to lekki i wszechstronny plugin dla serwerów Minecraft opartych na Paper/Spigot, który jest **wymagany** do działania wszystkich innych pluginów spod szyldu ZoneCode. Zapewnia podstawowe funkcje zarządzania serwerem, takie jak wyświetlanie informacji o serwerze, przeładowanie konfiguracji oraz sprawdzanie aktualizacji. Plugin integruje się również z bStats w celu zbierania anonimowych statystyk użytkowania.

## Funkcje

- **Komenda informacyjna**: Użyj `/zonecode`, aby wyświetlić informacje o serwerze z brandingiem ZoneCode, w tym dane o autorach, stronie internetowej i serwerze Discord.
- **Komenda pomocy**: Uruchom `/zonecode help`, aby zobaczyć listę dostępnych komend, dostosowaną do uprawnień użytkownika.
- **Przeładowanie pluginu**: Przeładuj konfigurację pluginu za pomocą `/zonecode reload` bez konieczności restartowania serwera.
- **Automatyczne aktualizacje**: Sprawdź i zainstaluj najnowszą wersję pluginu za pomocą `/zonecode update`
- **Konfigurowalne komunikaty**: Dostosuj prefiksy komunikatów i inne ustawienia w pliku `config.yml`.
- **Wsparcie dla uprawnień**: Precyzyjne uprawnienia do kontroli dostępu do komend (`zonecode.use`, `zonecode.reload`, `zonecode.update`, `zonecode.autoupdater`).

## Wymagania

- **Serwer Minecraft**: Paper lub Spigot (KAŻDA WERSJA).
- **Java**: Wersja 8 lub wyższa.

## Komendy

| Komenda | Opis | Uprawnienie |
| --- | --- | --- |
| `/zonecode` | Wyświetla informacje o serwerze od ZoneCode. | `zonecode.use` |
| `/zonecode help` | Pokazuje listę dostępnych komend. | `zonecode.use` |
| `/zonecode reload` | Przeładowuje konfigurację pluginu. | `zonecode.reload` |
| `/zonecode update` | Sprawdza i instaluje aktualizacje pluginu. | `zonecode.update` |
| `/zonecode autoupdater on/off` | Samoistnie instaluje nowe aktualizacje pluginu (można tą opcje wyłączyć). | `zonecode.autoupdater` |

**Aliasy**: `/developer`, `/dev`, `/development`

## Uprawnienia

- `zonecode.use` (domyślnie: true): Pozwala na użycie komend `/zonecode` i `/zonecode help`.
- `zonecode.reload` (domyślnie: op): Pozwala na użycie komendy `/zonecode reload`.
- `zonecode.update` (domyślnie: op): Pozwala na użycie komendy `/zonecode update`.

## Konfiguracja

Plugin generuje plik `config.yml` w folderze `plugins/ZoneCode-API/` z następującymi domyślnymi ustawieniami:

```yaml
# Konfiguracja ZoneCode-API
version: 1.3
message-prefix: "§5[ZoneCode] §r"
```

Możesz zmodyfikować `message-prefix`, aby dostosować prefiks komunikatów wyświetlanych przez plugin.

## Wsparcie

- **Strona internetowa**: zonecode.dev
- **Discord**: dc.zonecode.dev
- **Problemy**: Zgłaszaj błędy lub sugestie na stronie.

## Licencja

Projekt jest licencjonowany na licencji MIT. Zobacz plik LICENSE dla szczegółów.

## Podziękowania

Stworzone przez ZoneCode Team. Dziękujemy za korzystanie z ZoneCode-API! Ten plugin jest wymagany do działania wszystkich innych pluginów od ZoneCode.
