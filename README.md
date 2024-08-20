# Oesia Mobile Automation Framework

Este proyecto es un framework de automatización de pruebas para dispositivos Android basado en Appium y Selenium. Está diseñado para implementar pruebas BDD usando la librería Behave y generar reportes detallados con Allure. El proyecto sigue las mejores prácticas de nomenclatura y organización de directorios para Python.

## Estructura del Proyecto

```plaintext
oesia-fwk/
├── src
│   ├── data/
│   │   ├── devices/                      > archivos JSON con las capabilities de los dispositivos
│   │   │   └── brand_devices_n.json
│   │   └── locators/                     > archivos JSON con los localizadores para los elementos de la UI
│   │       └── brand_locator_n.json
│   └── pages/
│       └── android/                      > implementaciones de Page Objects específicas para la plataforma Android
│           ├── calls/
│               └── call_page_n.py
│           ├── msn/
│               └── msn_page_n.py
│           └── browsers/
│               └── browsers_page_n.py
├── features/                             > directorio que contiene los archivos .feature y las Steps Definitions
│   ├── enviroment.py
│   ├── storage_tests/                    > directorio que contiene los archivos .feature escritos en Gherkin
│   │   ├── scenario_n.feature
│   │   └── scenario_outline_n.feature
│   └── steps/                            > directorio que contiene los archivos .feature escritos en Gherkin y las Steps Definitions
│       └── others_steps_n.py
├── reports/                              > directorio donde se almacenan los reportes y logs
│   ├── allure/
│       └── yyyymmdd_HHmmss.html
│   └── logs/
│       └── yyyymmdd_HHmmss.log
├── base/                                 > contiene clases base y utilidades comunes para la ejecución de pruebas
│   ├── base_page.py
│   ├── drivers.py
│   └── utils/
│       ├── common_utils.py
│       ├── custom_logger.py
│       └── appium_utils.py
├── configs/                              > archivos de configuración que permiten ajustar parámetros y configuraciones de pruebas
│   ├── config.json
│   └── settings.py
├── venv/                                 > entorno virtual de Python para gestionar las dependencias del proyecto
├── README.md
└── requirements.txt
```

### Requisitos previos
1. Python 3.8 o superior
2. Node.js y npm
3. OpenJDK
4. Appium Server
5. Appium Inspector
6. Configurar las variables de entorno

## Instalacion del proyecto
1. Clonar el repositorio
 - `git clone https://{PATH}/{PROJECT}.git`
2. Crear y activar un entorno virtual
- `python -m venv venv`
- `venv\Scripts\activate`
3. Instalar las dependencias
 - `pip install -r requirements.txt`


