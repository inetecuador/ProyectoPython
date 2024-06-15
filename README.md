
# Scraping Web de Productos

Este proyecto consiste en dos programas, el primero realiza scraping de un sitio web para obtener información de productos en venta, limpia y guarda la información en un archivo CSV. El segundo programa lee el archivo CSV, analiza los datos y los guarda en otro archivo CSV.

## Requisitos

- Python 3.7+
- pandas
- beautifulsoup4
- requests
- logging

## Instalación

Para instalar las dependencias ejecutar el siguiente comando:

````bash
pip install -r .\dep.txt
````

## Estructura de las carpetas.

````bash
ProyectoPython
|-- data/
|    |- processed/
|    |   |__ cleaned_products.csv    
|    |- raw/
|         |__ products.csv
|
|-- src/
|    |- analysis/
|        |__ __init__.py
|        |__ analysis.py
|        |- decorators/
|            |__ __init__.py
|            |__ decorators.py
|    |- scraping/
|        |__ __init__.py
|        |__ scraper.py
|__ dep.txt
|__ README.md
````

## Ejecución del Scraper

El scraper se ejecuta con el siguiente comando:

````bash
python .\src\scraping\scraper.py
````

Este comando genera el archivo "products.csv" en la carpeta "data\raw".

## Ejecución del análisis de datos

El análisis de datos se ejecuta con el siguiente comando:

````bash
python .\src\analysis\analysis.py
````


Este comando genera el archivo "cleaned_products.csv" en la carpeta "data\processed". 

