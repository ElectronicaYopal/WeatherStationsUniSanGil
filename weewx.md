# WeeWX: Aplicativo para recolección de datos.

WeeWX is a free, open source, software program, written in Python, which interacts with your weather station to produce graphs, reports, and HTML pages.
https://weewx.com/

## Instalación

Seguir los siguiente pasos para instalar en sistemas Debian, se puede encontrar aqui: http://weewx.com/docs/debian.htm

```bash
wget -qO - https://weewx.com/keys.html | sudo apt-key add -
wget -qO - https://weewx.com/apt/weewx-python3.list | sudo tee /etc/apt/sources.list.d/weewx.list
sudo apt-get update
sudo apt-get install weewx
```

Una vez instalado desplegará una interfaz de consola para añadir la estación.

## Información acerca de configuración de la estación (Vantage PRO2)

[weewx.conf](/weewx.conf)

### Información adicional

 - http://www.weewx.com/docs/usersguide.htm

 - https://www.weewx.com/docs/utilities.htm

