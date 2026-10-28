# Filtro ND 180°

Piccola web app (un solo file `index.html`, nessuna dipendenza) che consiglia il filtro ND da montare sul drone per mantenere la regola dei 180°.

## Uso

1. Scegli i fps del video (es. 60 → otturatore target 1/120).
2. Indica l'otturatore che il drone sceglierebbe in automatico senza filtro (ISO al minimo):
   - a mano, oppure
   - caricando una foto della scena scattata con l'app Fotocamera dell'iPhone e scelta dalla Libreria. L'app legge tempo, ISO e diaframma (EXIF) e stima l'otturatore del drone.
3. L'app mostra gli stop da togliere e l'ND consigliato (ND4 – ND256).

## Note

- Parametri del drone usati per la stima da foto: DJI Lito X1, diaframma f/1.7, ISO minimo 100 (costanti `DRONE_F` e `DRONE_ISO` in `index.html`).
- Le foto scattate direttamente dal selettore di Safari non contengono i dati EXIF: usare la Libreria.
- La stima da foto può differire di circa mezzo stop dal valore reale del drone.

## Pubblicazione

GitHub Pages: Settings → Pages → Branch `main`, cartella `/ (root)`.
