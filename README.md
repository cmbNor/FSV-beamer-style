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
   \usetheme{FSV}
   ```

   🔑 Merk: Dersom du vil slippe å kopiere `.sty` til hver prosjektmappe, kan du heller legge til hele repo-mappa som en **local TeX directory** i MiKTeX/TeX Live. Se dokumentasjonen i repo for hvordan du legger til path.

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
- Bilder
- TikZ-grafikk
- Eksempel på `\pause` (gradvis fremvisning)
- Eksempel på `\note` (presentasjonsnotater, støttet i Pympress)

---

## 💡 Tips

### Bruke Pympress som presentasjonsverktøy

For å vise Beamer-presentasjoner anbefales **Pympress**:

- Open source, fungerer på Windows, Linux og macOS
- Gir **presenter view** med:
  - Neste slide
  - Notater (`\note` i LaTeX)
  - Timer/klokke
- Mulighet for gradvis visning av punkter med `\pause`

📥 Last ned her: [https://pypi.org/project/pympress/](https://pypi.org/project/pympress/)

---

## 📚 Krav

- **LaTeX-distribusjon** (TeX Live eller MiKTeX anbefales)
- **XeLaTeX eller LuaLaTeX** for fontstøtte
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
