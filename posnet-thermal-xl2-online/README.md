# POSNET Thermal XL2 Online — opis sprzętu

Statyczna strona (jeden plik `index.html` + zdjęcia) opisująca wyrejestrowane drukarki
POSNET Thermal XL2 Online i możliwości ponownego wykorzystania ich niefiskalnych
podzespołów. Materiał do konsultacji z elektronikami.

## Zawartość

- `index.html` — samodzielna strona (bez zależności poza Google Fonts).
- `img/` — zdjęcia (zmniejszone, bez danych EXIF; numery seryjne zamazane).
- `robots.txt` + `vercel.json` — blokada indeksowania przez wyszukiwarki.

## Prywatność / indeksowanie

Strona ma być dostępna pod linkiem, ale **nie indeksowana** przez wyszukiwarki:
- `index.html` zawiera `<meta name="robots" content="noindex, nofollow">`,
- `vercel.json` ustawia nagłówek `X-Robots-Tag: noindex, nofollow`,
- `robots.txt` blokuje roboty.

Uwaga: samo repozytorium na GitHub jest publiczne — kod źródłowy jest widoczny dla
każdego, kto zna link lub znajdzie go w wyszukiwarce GitHuba. Blokada dotyczy
hostowanej strony, nie repozytorium.

## Hosting na Vercel

Przy tworzeniu projektu w Vercel ustaw **Root Directory** na
`posnet-thermal-xl2-online`. Framework: „Other” (strona statyczna, bez builda).
