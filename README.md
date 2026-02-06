```
           _                    _       
  o __  _ (_| o __  _  __ \/   |_) _ __ 
  | |||(_|__| | | |(_| |  /    |  (/_| |


```

### METAFONT VORLAGE FÜR WORKSHOP *IMAGINARY PEN*

HILFREICHE WERKZEUGE:
- Erstellung eines Proof PDFs

```
mktextfm gray;
mf-nowin --interaction=nonstopmode index;
gftodvi index.2602gf;
dvipdfmx -p a4 index.dvi; 
```

- Metafont zu OpenType

```
fontforge -lang=py -script mf2outline.py index.mf --fontname regular --familyname imaginarypen --fullname-as-filename --fullname imaginarypen-regular 
```

Voraussetzungen
- [Homebrew](https://brew.sh "Homebrew"), Paketverwaltung für Kommandozeilen-Tools
- [FontForge](https://formulae.brew.sh/formula/fontforge "FontForge"), Open-Source Schriftbearbeitungsprogramm mit Skript-Funktionen
- [mf2outline](https://github.com/linusromer/mf2outline "mf2outline"), Python-Skript, das METAFONT Schriftarten in Outline-Formate wie OpenType konvertiert
