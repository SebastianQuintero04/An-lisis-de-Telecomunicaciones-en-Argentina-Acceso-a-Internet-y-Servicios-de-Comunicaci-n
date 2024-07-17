# Análisis de Telecomunicaciones en Argentina
![Portada](./assets/portada.png)

## Índice
- [Introducción](#introducción)
- [Fuente de Datos](#fuente-de-datos)
- [Metodología](#metodología)
  - [Extracción, Transformación y Carga (ETL)](#extracción-transformación-y-carga-etl)
  - [Análisis Exploratorio de Datos (EDA)](#análisis-exploratorio-de-datos-eda)
  - [Definición y Seguimiento de KPIs](#definición-y-seguimiento-de-kpis)
  - [Desarrollo de Dashboard](#desarrollo-de-dashboard)
- [ Conlusiones y recomendaciones](#Conlusiones-y-recomendaciones)
- [Repositorio de GitHub](#repositorio-de-github)
- [Autor](#autor)

## Introducción

Este proyecto tiene como objetivo realizar un análisis exhaustivo del sector de las telecomunicaciones en Argentina, centrándose especialmente en el acceso a internet y otros servicios de comunicación. El propósito principal es proporcionar información estratégica que permita a una empresa prestadora de servicios mejorar la calidad de sus ofrecimientos, identificar oportunidades de expansión y diseñar soluciones personalizadas para sus clientes potenciales.

El análisis abarcará diversos aspectos del panorama de las telecomunicaciones en Argentina, incluyendo la disponibilidad y penetración de la fibra óptica, la distribución de tecnologías de acceso en diferentes regiones y el análisis de velocidades de conexión promedio. Estos datos no solo ayudarán a comprender el comportamiento actual del sector, sino que también servirán como base para la toma de decisiones estratégicas orientadas a mejorar la infraestructura y los servicios de comunicación en todo el país.

Este proyecto ha sido encargado por una empresa líder en el sector de las telecomunicaciones, con el objetivo de mantenerse a la vanguardia en la provisión de servicios innovadores y de alta calidad en un mercado dinámico y competitivo como el argentino.
## Fuente de Datos

Los datos utilizados en este análisis se encuentra en la carpeta [`Data`](./Data).

## Metodología

Para llevar a cabo este proyecto, se siguieron los siguientes pasos:

### Extracción, Transformación y Carga (ETL)
Se realizó un proceso de ETL para preparar los datos antes del análisis. Esto incluyó la extracción de los datos desde las fuentes originales, la limpieza y transformación de los mismos para garantizar su calidad y consistencia, y finalmente, la carga de los datos procesados en una base de datos para su posterior uso. El proceso de ETL se encuentra detallado en el archivo [`ETL.ipynb`](./ETL.ipynb).

### Análisis Exploratorio de Datos (EDA)
Se realizó un análisis exhaustivo de los datos utilizando Python y las librerías pandas, numpy y matplotlib en un notebook de Jupyter. Durante este proceso, se llevaron a cabo las siguientes tareas:
- Búsqueda y tratamiento de valores faltantes, atípicos y duplicados.
- Análisis de la distribución de las variables y su relación con los siniestros viales.
- Generación de visualizaciones coherentes para una mejor comprensión de los datos.
- Documentación detallada de los hallazgos y conclusiones en cada etapa del análisis.

El análisis exploratorio de datos se encuentra en el archivo [`EDA.ipynb`](./EDA.ipynb).

![Análisis Exploratorio de Datos](./assets/EDA.png)

### Definición y Seguimiento de KPIs
Antes de desarrollar el dashboard, se establecieron tres Key Performance Indicators (KPIs) para medir el progreso en la reducción de víctimas fatales en siniestros viales:
- 
KPI de Mejora Necesaria en Acceso a Internet:
Este indicador nos permitirá entender cuánto necesita mejorar cada provincia para alcanzar un objetivo de tasa de cambio del 2% en el acceso a Internet. Calcularemos este KPI trimestralmente utilizando datos del dataset 1, comparando la tasa de cambio actual con el objetivo establecido. se encuentra en [`kpi1.csv`](./assets/kpi1.csv).
- KPI de Distribución de Tecnologías de Acceso por Provincia:
En este análisis, evaluaremos la disponibilidad y penetración de la fibra óptica en diferentes localidades utilizando datos combinados de los datasets 1. Este KPI nos ayudará a medir la extensión de la cobertura y la intensidad de uso de este servicio crucial de comunicaciones.. El archivo relacionado a este KPI se encuentra en [`kpi2.csv`](./assets/kpi2.csv).
-KPI de Proporción de Población con Acceso a Fibra Óptica por Provincia>
Evaluaremos la disponibilidad y penetración de la fibra óptica en diferentes localidades utilizando datos combinados de el data set 2. Este KPI nos ayudará a medir la extensión de la cobertura y la intensidad de uso de este servicio crucial de comunicaciones.. El archivo relacionado a este KPI se encuentra en [`kpi3.csv`](./assets/kpi3.csv).

![KPIs](./assets/KPIs.png)

### Desarrollo de Dashboard
Se creó un dashboard interactivo utilizando la herramienta Power BI para presentar los principales insights de forma clara y accesible. Los KPIs definidos anteriormente se implementaron en el dashboard para su seguimiento. Además, el dashboard incluye:
- Filtros para explorar los datos según diferentes criterios (fecha, tipo de siniestro, características de las víctimas, etc.).
- Gráficos y visualizaciones que facilitan la interpretación de la información.
- Un diseño intuitivo y estéticamente agradable para mejorar la experiencia del usuario.

El archivo del dashboard se encuentra en la carpeta [`Dashboard.pbix`](./Dashboard.pbix).

## Conlusiones y recomendaciones

A través del análisis exploratorio de datos, la definición de KPIs y la visualización en el dashboard, se obtuvieron los siguientes resultados clave en relación a los siniestros viales de la Ciudad de Buenos Aires durante el periodo 2016-2021:

### Conclusiones

Disparidades Regionales: Existe una clara variabilidad en la infraestructura de telecomunicaciones entre las provincias argentinas. Algunas regiones muestran una mejor cobertura y acceso a tecnologías avanzadas como la fibra óptica, mientras que otras enfrentan desafíos significativos en términos de disponibilidad y calidad de los servicios.
Necesidad de Inversión: La infraestructura de telecomunicaciones requiere inversiones continuas para mejorar la cobertura y la calidad del servicio en todo el país. Esta inversión es crucial para apoyar el desarrollo económico, social y tecnológico, así como para garantizar la igualdad de acceso a las comunicaciones digitales.
Importancia de la Conectividad: En un mundo cada vez más digitalizado, la conectividad rápida y confiable es fundamental para el acceso a la educación, la salud, el comercio electrónico y el desarrollo de negocios. Mejorar la infraestructura de telecomunicaciones no solo promueve la inclusión digital, sino que también impulsa la innovación y la competitividad económica.
Regulación y Políticas Públicas: Las políticas y regulaciones adecuadas juegan un papel crucial en el desarrollo y la gestión eficiente de las telecomunicaciones. Es importante implementar marcos regulatorios que fomenten la inversión privada en infraestructura, al tiempo que protejan los intereses de los consumidores y promuevan la competencia en el mercado.
Desafíos Futuros: A medida que avanza la tecnología y aumenta la demanda de datos, surgirán nuevos desafíos en términos de capacidad de red, seguridad cibernética y gestión sostenible de recursos. Abordar estos desafíos requerirá una planificación estratégica a largo plazo y colaboración entre el sector público y privado.
En conclusión, las telecomunicaciones en Argentina enfrentan una serie de desafíos y oportunidades significativas. Mejorar la infraestructura y la regulación, así como promover la inclusión digital, son aspectos clave para asegurar que todos los ciudadanos puedan beneficiarse plenamente de las ventajas de la era digital.

### Recomendaciones

Inversión en Infraestructura: Promover y facilitar la inversión tanto pública como privada en infraestructura de telecomunicaciones es fundamental. Esto incluye la expansión de la cobertura de fibra óptica y la mejora de la red de transporte de datos para garantizar una conectividad rápida y confiable en todo el país.

Políticas de Inclusión Digital: Implementar políticas que fomenten la inclusión digital, especialmente en áreas rurales y menos desarrolladas, es crucial. Esto puede incluir subsidios para la instalación de infraestructura en áreas menos rentables económicamente y programas de capacitación digital para mejorar las habilidades de la población.

Regulación Eficaz: Mantener un marco regulatorio claro y eficaz que fomente la competencia en el mercado de las telecomunicaciones, proteja los derechos de los consumidores y promueva la innovación. La regulación también debe adaptarse rápidamente a los avances tecnológicos para garantizar un entorno justo y competitivo.

Seguridad Cibernética: Fortalecer las medidas de seguridad cibernética para proteger la infraestructura crítica de telecomunicaciones contra ciberataques y asegurar la privacidad de los datos de los usuarios. Esto es especialmente importante dado el aumento de la digitalización y el intercambio de información sensible a través de redes.

Desarrollo de Capacidades: Invertir en la formación y capacitación de profesionales en tecnologías de la información y comunicación (TIC). Esto no solo apoya la innovación tecnológica local, sino que también crea oportunidades de empleo y fortalece el capital humano en el sector de las TIC.

Colaboración Público-Privada: Fomentar la colaboración entre el sector público y privado para desarrollar soluciones innovadoras y sostenibles en telecomunicaciones. Esta colaboración puede facilitar la implementación de proyectos a gran escala y la mejora continua de la infraestructura y servicios.

## Repositorio de GitHub

El presente repositorio contiene los siguientes archivos y carpetas:

- [`Data`](./Data/): Carpeta con los archivos de datos originales proporcionados por el OMSV.
- [`CleanData`](./CleanData/): Carpeta con los datos limpios y procesados.
- [`ETL.ipynb`](./notebooks/ETL.ipynb): Archivo ETL.
- [`EDA.ipynb`](./notebooks/EDA.ipynb): Archivo EDA.
- [`Dashboard`](./Dashboard/): Carpeta con los archivos relacionados al dashboard desarrollado en Power BI.
- [`assets`](./assets/): Carpeta con imágenes y gráficos generados durante el análisis.
- [`README.md`](./README.md): Este archivo, que proporciona una descripción general del proyecto y sus resultados.

## Autor

Este proyecto fue desarrollado por Sebastian Quintero como parte de una iniciativa del Observatorio de Movilidad y Seguridad Vial de la Ciudad de Buenos Aires.

- LinkedIn: [www.linkedin.com/in/sebastian-quintero0413](https://www.linkedin.com/in/sebastian-quintero0413)
- Correo electrónico: [quinterosebastian820@gmail.com](mailto:quinterosebastian820@gmail.com)

Espero que los análisis y recomendaciones presentados en este proyecto contribuyan a la toma de decisiones informadas por parte de la empresa prestadora de servicios de telecomunicaciones. Estos insights están diseñados para mejorar la calidad de los servicios ofrecidos, identificar oportunidades de crecimiento y desarrollar soluciones personalizadas que satisfagan las necesidades de los clientes en el dinámico mercado de las telecomunicaciones en Argentina.
