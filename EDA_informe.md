Este proyecto tiene como objetivo:
Consultar los ingresos en las diversas áreas del sector de telecomunicaciones. De ese modo ver qué subsectores han crecido y cuáles han decrecido. Con el fin de poder invertir en el desarrollo del que dispone mayor crecimiento.


## `Selección de Datasets`
---
Todos los datasets a continuación, _excepto el principal_, poseen datos concerniente a ingresos. 

### Datasets a utilizar:
- Internet_Penetracion.csv  (`principal`)
- Internet_Ingresos.csv
- Telefonia_movil.csv
- Telefonia_fija.csv
- Television.csv

## `EDA`
---
- **_Internet_Penetracion.csv_** 
En la columna "Accesos por cada 100 hogares" se intercambió la coma por el punto en los registros.
Y a la vez se transformó a un valor numérico, para poder hacer los cálculos necesarios.

- **_Internet_Ingresos.csv_** 
En la columna "Ingresos (miles de pesos)" se removió el punto (.) en los registros. Y al mismo tiempo se transformaron los registros a valores numéricos.

- **_Telefonia_movil.csv_** 
En la columna "Ingresos (miles de \$)" se removió el punto (.) y el signo de dólar ($) de los registros. Y se transformaron a valores de tipo numérico.

- **_Telefonia_fija.csv_** 
En la columna "Ingresos (miles de $)" se removió el punto (.) como separador de miles y se intercambió la coma (,) por el punto(.) como separador de decimales en los registros, para luego poder convertir la columna entera a valores numéricos.

- **_Television.csv_** 
En la columna "Ingresos TV por suscripción (miles de \$)" se removió el punto (.) y el signo de dólar ($) de los registros. Y se transformaron a valores de tipo numérico. También en la columna "Ingresos TV satelital (miles de \$)" se removió el punto(.) y el signo de dólar (\$) de los registros. Y se transformaron a valores de tipo numérico. 

El paso a paso de los cambios enunciados arriba se incluyen en el archivo [step_by_step_EDA.ipynb](./step_by_step_EDA.ipynb)

## `Datos para Dashboard`
---
Cada dataset revisado y modificado se guardó en una carpeta llamada: **data_powerbi**. La cual es utilizada para crear el dashboard ya que contiene los registros limpios y transformados.

Los nuevos datasets son:

- internet_penetracion.csv
- ingresos_internet.csv
- ingresos_telefonia_movil.csv
- ingresos_telefonia_fija.csv
- ingresos_television.csv