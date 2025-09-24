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

prosjekter/
├── presentasjon/ # her ligger .tex-filene dine
└── fsv-style/ # her ligger beamerthemeFSV.sty

r
Kopier kode

2. **Koble stilfila til presentasjonen.**  
Øverst i `.tex`-dokumentet legger du inn:

```latex
\documentclass{beamer}
\usepackage{../fsv-style/beamerthemeFSV}
🔑 Merk: ../ betyr "gå ett nivå opp i mappestrukturen".
Hvis du har stilfila i samme mappe som presentasjonen kan du skrive:

latex
Kopier kode
\usepackage{beamerthemeFSV}
Kompiler med XeLaTeX eller LuaLaTeX.
Eksempel i terminal:

bash
Kopier kode
xelatex eksempelPresentasjon.tex