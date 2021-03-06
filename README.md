# Estaciones Meteorológicas

Estaciones meteorológicas con enlace de radio + almacenamiento en base de datos + plataforma web de visualización de datos históricos.

Se presentan dos modelos de estación:

- [Modelo Vantage](#vantage-pro2)
- [:sparkles: Red de estaciones propias :sparkles:](#red-de-estaciones-meteorológicas-lora)

## Vantage PRO2

Estación meteorológica de [**Davis Instruments**](https://www.davisinstruments.com/), empresa líder mundial en el desarrollo y fabricación de sistemas, sensores y equipos para la monitorización meteorológica. 

<img alt="Vantage PRO2" src="https://raw.githubusercontent.com/ElectronicaYopal/WeatherStationsUniSanGil/main/imgs/Vantage.jpg" width=30% height=30%>

### Descripción:

La estación cuenta con:
- sensor de humedad y temperatura
- sensor de radiación solar
- sensor velocidad y dirección de viento
- sensor pluviómetro de doble cubeta basculante
- panel solar y batería
- transmisor de radio
- receptor de radio y datalogger

Se encuentra ubicada en Campus Unisangil,Yopal a 374 metros sobre el nivel del mar.
[Ver en google maps](https://goo.gl/maps/FxejaJAe9rZrjSYg6)

El receptor de radio cuenta con datalogger y este a su vez está conectado vía USB a un servidor local.

### Acceso a los datos de la estación:

Para acceder a visualizar los datos de la estación ingresar al siguiente enlace: https://electronicayopal.github.io/Servicios/

Y hacer clic en la opción: :ballot_box_with_check: **Estación Meteorológica Unisangil**

**Nota:** *Para compatir el enlace, únicamente usar el indicado previamente* :point_up:

![View dashboard](/imgs/viewgrafana.gif)
*- Inicio de sesión no requerido.*

### Descargar datos

Para descargar los datos seleccione el rango de tiempo del cual desea realizar copia de los datos, y proceda a realizar como se muestra:

![Get data](/imgs/getdata.gif)

Los datos se descargan en un archivo *.csv* y se puede abrir con *excel*, las columnas están delimitadas por comas y los números decimales con punto.
La primera o segunda fila del archivo indica los nombres de las columnas y las unidades de los datos.

Para una correcta visualización al abrir el archivo es importante:
 - Delimitar las columnas únicamente por coma ","; *por defecto está delimitado así para excel*
 - Una vez estrucurado el archivo en excel, si los números no son operables, es necesario cambiar los puntos "." por coma ","

![View data excel](/imgs/dataexcel.gif)

*Para abrir el cuadro de busqueda y reemplazar presione:* [Ctrl]+[B]
______

## Red de Estaciones Meteorológicas LoRa

En desarrollo...

______
## InfoConfig

1. [MariaDB](/MariaDB.md)
2. [WeeWX](/weewx.md)
3. [Grafana](/Grafana.md)
4. [Dashboard](/ConfigDashboard.md)
