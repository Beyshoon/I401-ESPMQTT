# I401-ESPMQTT

## Descripción

Sistema IoT desarrollado con ESP32, MQTT, Flask y Supabase para controlar un semáforo desde una interfaz web y registrar automáticamente cada evento en una base de datos en la nube.

## Tecnologías utilizadas

- ESP32
- MQTT
- Flask (Python)
- Supabase
- HTML / CSS
- GitHub

## Funcionamiento

1. El usuario selecciona un color desde la página web.
2. Flask publica el mensaje mediante MQTT.
3. El ESP32 recibe la orden y cambia el estado del semáforo.
4. Flask registra el evento en Supabase con:
   - Estado
   - Dispositivo
   - Origen
   - Fecha y hora

## Base de datos

La tabla **registro_eventos** almacena:

- id
- created_at
- estado
- dispositivo
- origen

## Estructura del proyecto

```
I401-ESPMQTT/
│
├── app.py
├── templates/
│   └── index.html
├── capturas/
└── proyecto.zip
```

## Autor

Bastián Gutiérrez -
Jean Guerra

Ingeniería en Electrónica y Sistemas Inteligentes  
INACAP
