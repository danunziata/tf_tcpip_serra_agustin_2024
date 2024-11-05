# Prupuesta  

## Trabajo Final Aplicaciones TCP/IP

## Integrantes:
- Serra Agustin

## Digitalización de medidores en el borde con visión por computadora.

### Resumen:
El proyecto busca implementar un sistema de digitalización automática de medidores analógicos utilizando técnicas de visión por computadora en el borde (edge computing). Esta solución permitirá la lectura en tiempo real de instrumentos análogos existentes sin necesidad de reemplazarlos, modernizando así la infraestructura de medición de manera costo-efectiva.


### Introducción
La transformación digital de procesos industriales requiere la obtención de datos en tiempo real. Sin embargo, muchas instalaciones cuentan con instrumentos analógicos que, aunque funcionales, no permiten la captura automática de datos. Este proyecto propone una solución no invasiva basada en visión por computadora para digitalizar las lecturas de estos instrumentos, permitiendo su integración con sistemas modernos de monitoreo y análisis.

### Objetivos
- Plantear escenario de medición de un instrumento analógico.
- Lograr la digitalización del instrumento mediante visión por computadora.
- Persistir la información y visualizar los datos en tiempo real.


### Descripción de la Propuesta
El sistema consistirá en:
1. Modulo esp32-CAM para la captura de video y procesamiento de la imagen. En el módulo esp32-CAM se realizara:
    - Preprocesamiento de imágenes
    - Conversión a valores digitales
    - Exportación de datos.

Se va a utilizar como base el repositorio publico , el cual tiene como propuesta:

2. Sistema de almacenamiento de series temporales con InfluxDB.
3. Implementar broker MQTT.
4. Interfaz de visualización en tiempo real con Grafana o Streamlit.

A continuación se muestra la arquitectura de la solución para “n” instrumentos analogicos:


### Plan de Trabajo Tentativo
- **Fase 1:** Análisis y diseño de la aplicación.
- **Fase 2:** Armar escenario, configuración del dispositivo.
- **Fase 3:** Exportar las métricas a InfluxDB y visualizarlas en Grafana/Streamlit.
- **Fase 4:** Agregar broker mqtt.
- **Fase 5:** Dockerización.
- **Fase 6:** Despliegue en Kubernetes.
- **Fase 7:** Ajustes finales, corrección de errores y entrega.

### Referencias:
- [https://jomjol.github.io/AI-on-the-edge-device-docs/](https://jomjol.github.io/AI-on-the-edge-device-docs/)
- [https://danunziata.github.io/Aplicaciones_TCP_IP/](https://danunziata.github.io/Aplicaciones_TCP_IP/)
