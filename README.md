# ProyectoGesti-ndeDatosIA
# Motor de Notificaciones para Red Social

## Descripción del Proyecto

Sistema de notificaciones en tiempo real para una red social, diseñado para procesar eventos como likes, comentarios y nuevos seguidores, y enviar notificaciones push a los usuarios destino. El proyecto utiliza una arquitectura Pipeline Híbrido Modular que permite manejar grandes volúmenes de eventos y adaptarse rápidamente a cambios frecuentes en las funcionalidades.

## Arquitectura Seleccionada

**Pipeline Híbrido Modular**

- **Ingesta**: Apache Kafka – captura eventos en tiempo real.
- **Procesamiento**: Apache Spark Streaming – transforma los eventos y genera notificaciones.
- **Servicio**: API Gateway + Firebase Cloud Messaging (FCM) – expone la API y envía notificaciones push a dispositivos móviles.

La arquitectura es escalable (componentes desacoplados), segura (control de acceso por capa) e interoperable (uso de estándares y módulos independientes).
