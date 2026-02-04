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