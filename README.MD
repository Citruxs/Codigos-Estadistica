# Codigos-Estadistica

Repositorio con ejercicios, simulaciones y tareas de estadistica desarrollados principalmente en R Markdown, junto con un notebook en Julia. El material se enfoca en estimacion, simulacion de variables aleatorias, estadistica descriptiva y verificacion empirica de propiedades de estimadores.

## Contenido del repositorio

### Archivos principales

- `TM1_Est_ALC.Rmd`: estimacion puntual de parametros de una distribucion normal a partir de momentos poblacionales y comparacion entre estimadores.
- `Ej_1b_1c.Rmd`: analisis exploratorio de datos con estadisticas descriptivas y graficos para dos conjuntos de datos externos en formato CSV.
- `Consistencia de estimador de muestras con distribución normal.Rmd`: simulacion de muestras normales para estudiar la consistencia de estimadores de media y varianza.
- `T2_Estadistica.Rmd`: simulacion de variables aleatorias mediante aceptacion-rechazo y transformacion inversa, con verificacion de estimadores por momentos y maxima verosimilitud.
- `T2_estadística.ipynb`: version en Julia de una simulacion relacionada con aceptacion-rechazo y validacion de estimadores.

## Temas abordados

- Estadistica descriptiva
- Simulacion de distribuciones
- Metodo de momentos
- Estimacion por maxima verosimilitud
- Consistencia de estimadores
- Visualizacion de resultados

## Requisitos

### Para los archivos `.Rmd`

- R
- RStudio o un entorno compatible con R Markdown
- Paquete `tidyverse`
- Opcionalmente `rmarkdown` para generar HTML o PDF

Instalacion basica en R:

```r
install.packages(c("tidyverse", "rmarkdown"))
```

### Para el notebook `.ipynb`

- Julia
- Jupyter o Visual Studio Code con soporte para notebooks
- Paquetes de Julia:

```julia
using Pkg
Pkg.add(["Distributions", "LinearAlgebra", "Plots"])
```

## Como usar

### Ejecutar archivos R Markdown

1. Abre el archivo `.Rmd` en RStudio o VS Code.
2. Instala las dependencias si es necesario.
3. Ejecuta los chunks manualmente o compila el documento completo.

### Ejecutar el notebook de Julia

1. Abre `T2_estadística.ipynb` en Jupyter o VS Code.
2. Selecciona un kernel de Julia.
3. Ejecuta las celdas en orden.

## Observaciones importantes

- `Ej_1b_1c.Rmd` usa rutas locales de Windows para cargar los archivos `dias_perdidos.csv` y `Alturas.csv`. Para reproducir ese analisis en otro equipo, hay que reemplazar esas rutas por rutas relativas o disponer de los CSV en la ubicacion correcta.
- Algunos documentos estan pensados como tareas academicas y priorizan la demostracion del procedimiento estadistico sobre la estructura de un paquete reproducible.

## Objetivo del repositorio

Servir como coleccion de practicas y ejercicios de estadistica aplicada, utiles para estudiar tecnicas de simulacion, inferencia y analisis exploratorio con R y Julia.
