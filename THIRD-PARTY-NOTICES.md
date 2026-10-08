# Komponenty zewnętrzne

Ten sam spis (z pełnym tekstem licencji MIT Velopack) jest instalowany razem z aplikacją:
`%LOCALAPPDATA%\RollCam\current\THIRD-PARTY-NOTICES.txt`.

## FFmpeg

RollCam uruchamia program FFmpeg jako osobny proces. FFmpeg nie jest częścią instalatora: przy pierwszym
uruchomieniu aplikacja pobiera wersję **8.1.2 „full_build-shared”** przygotowaną przez Gyan Doshi:

- plik: <https://github.com/GyanD/codexffmpeg/releases/download/8.1.2/ffmpeg-8.1.2-full_build-shared.zip>
- SHA-256: `274923c68904a9b76c73b908f57923dafba81155856cd742138515ded570d066`
- informacje o wersjach: <https://www.gyan.dev/ffmpeg/builds/>

Ta wersja FFmpeg jest udostępniana na licencji **GNU GPL v3** (zawiera m.in. libx264). Tekst licencji jest w pliku
`LICENSE` obok pobranego programu (`%LOCALAPPDATA%\Nagrywarka\ffmpeg\8.1.2\LICENSE`). Kod źródłowy FFmpeg:
<https://ffmpeg.org/download.html#get-sources> (wydanie 8.1.2: <https://ffmpeg.org/releases/ffmpeg-8.1.2.tar.xz>).

FFmpeg is a trademark of Fabrice Bellard, originator of the FFmpeg project.

## Velopack

Instalator i aktualizacje (`Setup.exe`, `Update.exe`, `Velopack.dll`): [Velopack](https://github.com/velopack/velopack),
licencja [MIT](https://github.com/velopack/velopack/blob/main/LICENSE).
Copyright © 2021 Caelan Sayler, Copyright © 2024 Velopack Ltd.

## .NET

Aplikacja działa na [.NET 10 Desktop Runtime](https://dotnet.microsoft.com/download/dotnet/10.0) (licencja MIT),
który instalator doinstalowuje w razie potrzeby.
