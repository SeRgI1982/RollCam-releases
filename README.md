# RollCam

*[English below](#english)*

Nagrywanie ekranu na Windows: cały monitor, wybrane okno albo zaznaczony obszar, z mikrofonem i kamerą w rogu
(obraz w obrazie). Nagrywanie można wstrzymać, a przed zapisem obejrzeć, przyciąć, wykadrować, dodać napisy
i zapisać jako MP4, MKV, WebM, GIF, WebP albo AVIF.

To repozytorium zawiera tylko gotowe wersje do pobrania: instalator i paczki aktualizacji.

## Pobieranie

**[⬇ Pobierz RollCam (instalator dla Windows)](https://github.com/SeRgI1982/RollCam-releases/releases/latest/download/RollCam-win-Setup.exe)**

Wszystkie wersje i lista zmian: [Releases](https://github.com/SeRgI1982/RollCam-releases/releases).

## Wymagania

- Windows 10 (wersja 2004 lub nowsza) albo Windows 11, 64-bitowy.
- Około 450 MB miejsca na dysku (aplikacja, .NET i ffmpeg).
- Połączenie z internetem przy instalacji i pierwszym uruchomieniu.

Niczego nie trzeba instalować ręcznie ani ustawiać zmiennych środowiskowych.

## Instalacja

1. Pobierz i uruchom `RollCam-win-Setup.exe`.
2. Jeśli pojawi się okno „System Windows ochronił ten komputer”, kliknij **Więcej informacji**, a potem
   **Uruchom mimo to**. Instalator nie jest jeszcze podpisany cyfrowo, dlatego Windows go nie rozpoznaje.
3. Jeśli na komputerze nie ma środowiska **.NET 10 Desktop Runtime**, instalator pobierze je i zainstaluje
   (Windows może poprosić o zgodę administratora – tylko w tym kroku).
4. RollCam instaluje się dla bieżącego użytkownika (`%LOCALAPPDATA%\RollCam`) i dodaje skrót na pulpicie oraz w menu Start.

### Pierwsze uruchomienie

Do nagrywania i zapisu filmów RollCam używa programu [ffmpeg](https://ffmpeg.org). Jeśli na komputerze nie ma
zgodnej wersji, aplikacja przy pierwszym uruchomieniu sama pobierze go (ok. 100 MB) do
`%LOCALAPPDATA%\Nagrywarka\ffmpeg` i sprawdzi sumę kontrolną pliku. Później uruchamia się od razu.

## Aktualizacje

RollCam sam sprawdza w tle, czy jest nowa wersja, i pobiera ją. Instaluje się przy następnym uruchomieniu aplikacji,
więc nigdy nie przerywa nagrywania. Pobierane są tylko zmienione pliki.

## Odinstalowanie

**Ustawienia → Aplikacje → RollCam → Odinstaluj.** Usuwane są aplikacja, skróty i pobrany ffmpeg.
Ustawienia zostają w `%APPDATA%\Nagrywarka` – można usunąć ten folder ręcznie. Nagrania nie są usuwane.

## Gdzie są pliki

| Co | Gdzie |
|---|---|
| Aplikacja | `%LOCALAPPDATA%\RollCam` |
| ffmpeg | `%LOCALAPPDATA%\Nagrywarka\ffmpeg` |
| Ustawienia | `%APPDATA%\Nagrywarka\settings.json` |
| Nagrania | folder **Wideo** użytkownika (do zmiany w ustawieniach aplikacji) |

## Problemy i sugestie

Zgłoś je w [Issues](https://github.com/SeRgI1982/RollCam-releases/issues): opisz, co się stało, i dołącz wersję
Windows oraz RollCam.

## Licencja

RollCam jest darmowy i udostępniany na licencji [MIT](LICENSE.txt) (© 2026 DevGroup): „tak jak jest”, bez żadnych
gwarancji i bez odpowiedzialności autora za skutki używania programu.
Komponenty zewnętrzne mają własne licencje: [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).

---

## English

RollCam is a free screen recorder for Windows: a whole monitor, a window or a selected area, with a microphone and
a camera in the corner (picture-in-picture). You can pause, preview, trim, crop, add subtitles and save as MP4, MKV,
WebM, GIF, WebP or AVIF. The app follows the Windows display language (Polish or English); you can change it in
Settings.

**[⬇ Download RollCam (Windows installer)](https://github.com/SeRgI1982/RollCam-releases/releases/latest/download/RollCam-win-Setup.exe)**

- **Requirements:** Windows 10 (2004 or newer) or Windows 11, 64-bit; about 450 MB of disk space; an internet
  connection during installation and the first start.
- **Install:** run `RollCam-win-Setup.exe`. If Windows shows “Windows protected your PC”, click **More info** →
  **Run anyway** (the installer is not code-signed yet). If .NET 10 Desktop Runtime is missing, the installer
  installs it (Windows may ask for administrator consent for that step only).
- **First start:** RollCam downloads [ffmpeg](https://ffmpeg.org) (about 100 MB) once, unless a compatible one is
  already installed.
- **Updates** download in the background and install the next time the app starts.
- **Uninstall:** Settings → Apps → RollCam → Uninstall. Settings stay in `%APPDATA%\Nagrywarka`; recordings are kept.
- **License:** [MIT](LICENSE.txt), © 2026 DevGroup – free, provided “as is”, without warranty.
  Third-party components: [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).
- **Issues:** [GitHub Issues](https://github.com/SeRgI1982/RollCam-releases/issues).
