# ¿Quién tiene el poder en las provincias argentinas? Un Índice de Género, Decisión y Representación

<!-- CAMBIAR "https://place-hold.it/1920x1080" POR EL LINK A LA IMAGEN CORRESPONDIENTE -->
[![¿Quién tiene el poder en las provincias argentinas?](https://fund.ar/wp-content/uploads/2023/03/iStock-1393623109.jpg)](https://fund.ar/wp-content/uploads/2023/03/Fundar_Quien-tiene-el-poder-en-las-provincias-argentinas_CC-BY-NC-ND-4.0.pdf)

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%20NC%20SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
<!-- [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1234.svg)](https://zenodo.org/doi/10.5281/zenodo.11186044) -->


La desigualdad de género ha adquirido una visibilidad pública sin precedentes en los últimos años, convirtiéndose en un elemento clave en la planificación del desarrollo del país. Reconociendo la complejidad estructural de este fenómeno y su desafío para la política pública, desde [Fundar](https://fund.ar/) elaboramos un Índice Subnacional de Igualdad de Género (ISIG).

El ISIG aborda la desigualdad de género en las 24 jurisdicciones del país y consta de cuatro aspectos:

- Decisión y representación política
- Trabajo e ingresos
- Educación y oportunidades
- Salud y protección

Cada medida del ISIG utiliza indicadores construidos de manera sintética y agregada para ofrecer una comprensión integral de la situación de género en cada provincia.

Este repositorio contiene los archivos necesarios para el cálculo de la primera edición del ISIG: el [Índice de Género, Decisión y Representación](https://fund.ar/wp-content/uploads/2023/03/Fundar_Quien-tiene-el-poder-en-las-provincias-argentinas_CC-BY-NC-ND-4.0.pdf) (IGDR). El IGDR, creado por primera vez, sistematiza las desigualdades que existen entre géneros en las posibilidades de integrar las élites políticas, judiciales y económicas de cada provincia en Argentina, revelando las heterogeneidades entre las 24 jurisdicciones en el acceso al poder y la medida en que la representación por género difiere de una situación de paridad. 


## Datos del índice agregado

La arquitectura de este índice se basa en 7 indicadores agrupados en dos componentes. Estos dos componentes luego se agregan para constituir el Índice de Género, Decisión y Representación (IGDR), que está disponible para cada una de las 24 jurisdicciones de Argentina.

Para acceder a los resultados de los indicadores, los componentes y el índice, consultar [este enlace](https://github.com/datos-Fundar/Indice_genero_decision_representacion/tree/main/data/processed). Para acceder a los datos desagregados por género que informan el procesamiento, consultar [este enlace](https://github.com/datos-Fundar/Indice_genero_decision_representacion/tree/main/data/raw). 

El IGDR se operacionaliza de la siguiente manera: 

### Indicadores

- Poder Ejecutivo Municipal (PEM) se define como el cociente entre la proporción de  intendentas mujeres sobre la proporción de intendentes varones. Para CABA se consideran las presidencias de las juntas comunales. 

- Poder Ejecutivo Provincial (PEP) es un indicador compuesto definido por el cociente entre la proporción de ministras mujeres sobre la proporción de ministros varones en el gabinete provincial, junto al género de quien encabeza la gobernación provincial. El  peso asignado a la composición del gabinete es del 80% y el 20% restante a la gobernación, que impacta positivamente si es mujer.

- Poder Judicial Provincial (PJP) se define como el cociente entre la proporción de mujeres sobre la proporción de varones entre magistrados/as de las justicias ordinarias y ministras/os de los tribunales superiores de las provincias. 

- Liderazgo Privado (LP) se define como el cociente entre la proporción de MiPyMEs lideradas por mujeres sobre la proporción de MiPyMEs lideradas por varones. Se considera que el liderazgo es femenino en dos casos: (a) empresas que son personas físicas jurídicas cuya titular es mujer; (b) empresas que son personas jurídicas con un 51% de mujeres en su composición accionaria o con el 25% de la composición y al menos una mujer en el directorio. 

- Poder Legislativo Municipal (PLM) se define como el cociente entre la proporción de  mujeres sobre la proporción de varones en los concejos municipales. Para CABA se consideran las Juntas Comunales. 

- Poder Legislativo Provincial (PLP) se define como el cociente entre la proporción de  mujeres sobre la proporción de varones en los órganos legislativos provinciales. En los casos bicamerales, se considera la composición de la cámara baja. 

- Poder Partidario (PP) se define como el cociente entre la proporción de listas electorales al Congreso de la Nación encabezadas por mujeres sobre la proporción de listas encabezadas por varones. Para la Cámara de Diputados se considera la elección de 2021 y para el Senado las elecciones de 2017, 2019 y 2021. 

El IGDR mide brechas de género en todos los indicadores, para cada una de las jurisdicciones, con el fin de capturar relaciones desiguales de género. En todos los casos las brechas son el resultado del cociente entre valores femeninos y masculinos, que refleja la proporción de mujeres en relación con la de varones. Para asegurar comparabilidad se aplicó una estandarización de las proporciones respecto al punto de paridad, que puede ser del 50% o el valor inferior más cercano si los totales son impares. Los resultados de los ratios correspondientes fueron convertidos en una escala de 0-100, truncados en un punto de igualdad. 


### Componentes

Todos los indicadores recibieron igual ponderación y fueron agregados aritméticamente (promedio simple) para computar cada componente. 

- Poder de Decisión (Cpd) representa el cociente entre la suma de los indicadores de Poder Ejecutivo Municipal (PEM), Poder Ejecutivo Provincial (PEP), Poder Judicial Provincial (PJP) y Liderazgo Privado (LP), dividida por 4. 

- Representación Política (Crp) representa el cociente entre la suma de los indicadores de Poder Legislativo Municipal (PLM), Poder Legislativo Provincial (PLP) y Poder Partidario (PP), dividida por 3. 


### Índice de Género, Decisión y Representación

Para computar el IGTI, los componentes fueron agregados geométricamente, es decir como la raíz cuadrada del producto entre los componentes de Poder de Decisión (Cpd) y Representación Política (Crp).


## ¿Cómo citar?

```bibtex
@misc{cerra2023poder,
  author = {Cerra, María Emilia and Avenburg, Alejandro and Bergallo, Paola and Puglia, María de las Nieves and Risaro, Daniela Belén and Fernández Erlauer, Micaela and Argoitia, Juan Martin},  
  title = {¿Quién tiene el poder en las provincias argentinas? Un Índice de Género, Decisión y Representación},
  year = {2023},
  institution  = {Fundar},
  url = {https://fund.ar/wp-content/uploads/2023/03/Fundar_Quien-tiene-el-poder-en-las-provincias-argentinas_CC-BY-NC-ND-4.0.pdf},
}
```