# Oesia Mobile Automation Framework

Este proyecto es un framework de automatización de pruebas para dispositivos Android basado en Appium y Selenium. Está diseñado para implementar pruebas BDD usando la librería Behave y generar reportes detallados con Allure. El proyecto sigue las mejores prácticas de nomenclatura y organización de directorios para Python.

## Estructura del Proyecto

```plaintext
oesia-fwk/
├── src
│   ├── data/
│   │   ├── devices/
│   │   │   └── brand_devices_n.json
│   │   └── locators/
│   │       └── brand_locator_n.json
│   └── pages/
│       └── android/
│           ├── calls/
│               └── call_page_n.py
│           ├── msn/
│               └── msn_page_n.py
│           └── browsers/
│               └── browsers_page_n.py
├── features/
│   ├── enviroment.py
│   ├── storage_tests/
│   │   ├── scenario_n.feature
│   │   └── scenario_outline_n.feature
│   └── steps/
│       └── others_steps_n.py
├── reports/
│   ├── allure/
│       └── yyyymmdd_HHmmss.html
│   └── logs/
│       └── yyyymmdd_HHmmss.log
├── base/
│   ├── base_page.py
│   ├── drivers.py
│   └── utils/
│       ├── common_utils.py
│       ├── custom_logger.py
│       └── appium_utils.py
├── configs/
│   ├── config.json
│   └── settings.py
├── venv/
├── README.md
└── requirements.txt

### Requisitos previos
Python 3.8 o superior
Node.js y npm
OpenJDK
Appium Server
Appium Inspector
