# Carpeta de datos

Archivos ya incluidos en esta carpeta (pequeños, por eso sí se suben al repositorio):

- **`Variables_socioeconomicas.xlsx`** — variables socioeconómicas por Community Area
  (población, renta per cápita, tasa de desempleo, tasa de pobreza, nivel educativo),
  usado en `notebooks/03_modelo_final.ipynb`.

- **`Chicago_Health_Atlas_Community_Areas.csv`** — variables socioeconómicas por Community
  Area (renta per cápita, nivel educativo, % población, población total), usado en
  `notebooks/02_exploracion_modelos.ipynb` durante el proceso de exploración inicial.

Ambos provienen del [Chicago Health Atlas](https://chicagohealthatlas.org/).

**`chicago_crimes_2020_2024.csv`** no se incluye por su tamaño (~300 MB, por encima del
límite de subida de GitHub). Para obtenerlo:

1. Ve al [Chicago Data Portal — Crimes 2001 to present](https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2).
2. Filtra por fecha desde el 1 de enero de 2020 en adelante y exporta como CSV. Si el archivo
   incluye también los primeros días de 2025, no supone un problema: ese filtrado adicional
   se realiza dentro de `01_eda.ipynb`.

> ⚠️ **Importante:** el archivo se descargará con otro nombre (por ejemplo,
> `Crimes_-_2001_to_Present.csv`). Renómbralo exactamente a **`chicago_crimes_2020_2024.csv`**
> antes de guardarlo en esta carpeta — los notebooks buscan ese nombre concreto y no
> funcionarán si el archivo se llama de otra forma.

Ver la sección "Datos" del README principal para más detalles.
