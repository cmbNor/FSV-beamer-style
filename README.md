# FSV Beamer Theme

Dette repoet inneholder en egen **Beamer stilfil** (`beamerthemeFSV.sty`) med farger og oppsett tilpasset Fagskolen Viken.  
Formålet er å sikre at alle presentasjoner får en enhetlig profil.

---

## 📦 Innhold

- `beamerthemeFSV.sty` – selve stilfila.
- `eksempelPresentasjon.tex` – en enkel LaTeX-presentasjon som viser hvordan temaet brukes.
- `README.md` – denne veiledningen.

---

## 🚀 Kom i gang

1. **Plasser mappen med stilfila et sted på maskinen din.**  
   For eksempel:

   ```
   prosjekter/
   ├── presentasjon/   # her ligger .tex-filene dine
   └── fsv-style/      # her ligger beamerthemeFSV.sty
   ```

2. **Koble stilfila til presentasjonen.**  
   Øverst i `.tex`-dokumentet legger du inn:

   ```latex
   \documentclass{beamer}
   \usepackage{../fsv-style/beamerthemeFSV}
   ```

   🔑 Merk: `../` betyr "gå ett nivå opp i mappestrukturen".  
   Hvis du har stilfila i samme mappe som presentasjonen kan du skrive:

   ```latex
   \usepackage{beamerthemeFSV}
   ```

3. **Kompiler med XeLaTeX eller LuaLaTeX.**  
   Eksempel i terminal:

   ```bash
   xelatex eksempelPresentasjon.tex
   ```

---

## 🖼️ Eksempelpresentasjon

Det følger med en fil `eksempelPresentasjon.tex` som demonstrerer:

- Slides med ren tekst
- Punktlister
- Bilde
- TikZ-grafikk
- Tips-slide om **Sumatra PDF**

Dette gir et utgangspunkt for å bygge egne presentasjoner.

---

## 💡 Tips

### Bruke LLM for å lage slides

Store språkmodeller (LLM), som ChatGPT, kan være et nyttig verktøy for å generere utkast til presentasjoner.  
Hvis du gir modellen teksten eller disposisjonen du vil ha inn i en presentasjon, kan den automatisk foreslå LaTeX-kode for slides.  
Resultatet blir ofte et godt utgangspunkt som du senere kan justere.


### PDF-leser med presentasjonsmodus

Beamer lager vanlige PDF-filer. Du kan bruke hvilken som helst PDF-leser for å vise dem.  
Et godt gratis-alternativ (særlig på Windows) er:

- **Sumatra PDF**  
  Lettvekts, open source PDF-leser med en enkel og god presentasjonsmodus.  
  Last ned her: [https://www.sumatrapdfreader.org/](https://www.sumatrapdfreader.org/)

---

## 📚 Krav

- **LaTeX-distribusjon** (TeX Live eller MikTeX anbefales)
- **XeLaTeX eller LuaLaTeX** for å støtte fontvalg via `fontspec`
- Følgende pakker må være installert:
  - `tikz`
  - `graphicx`
  - `xcolor`
  - `etoolbox`
  - `siunitx`

---

## 🏫 Lisens og bruk

Dette temaet er laget for **Fagskolen Viken**.  
Andre kan bruke det som mal eller tilpasse det etter behov.
