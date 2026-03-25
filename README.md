# App de Turismo con QR y Geolocalización - Flutter

## Descripción General
Este proyecto consiste en el desarrollo de una aplicación móvil en Flutter orientada al turismo, la cual permite a los usuarios interactuar con puntos de interés mediante el escaneo de códigos QR.

La aplicación está diseñada para ofrecer una experiencia dinámica donde usuarios (especialmente turistas) puedan descubrir lugares relevantes de una ciudad, visualizar su ubicación en el mapa y acceder a contenido adicional como enlaces web.

---

## Demo

[![Ver demo](https://img.youtube.com/shorts/lVxoGPh3P7c/0.jpg)](https://youtube.com/shorts/lVxoGPh3P7c)

---

## Objetivo del Proyecto
Implementar una aplicación móvil que integre múltiples funcionalidades clave de desarrollo en Flutter, tales como:

- Lectura de códigos QR
- Geolocalización
- Visualización de mapas
- Persistencia de datos local y remota
- Integración con APIs

---

## Enfoque del Proyecto
La idea principal del proyecto es simular un sistema turístico interactivo donde la ciudad cuente con puntos físicos con códigos QR.  

Al escanear estos códigos, el usuario puede:
- Obtener información del lugar
- Visualizar su ubicación en el mapa
- Acceder a contenido externo relacionado

Este enfoque busca mejorar la experiencia turística mediante el uso de tecnología móvil.

---

## Funcionalidades Implementadas

### Autenticación
- Inicio de sesión requerido para acceder a la lectura de QR
- Asociación de acciones al usuario autenticado

---

### Lectura de QR
- Escaneo de códigos QR desde la aplicación
- Soporte para:
  - Coordenadas geográficas (`geo`)
  - URLs (`http`)

---

### Visualización en Mapas
- Integración con Google Maps
- Visualización del punto geográfico obtenido desde el QR

---

### Geolocalización
- Obtención de la ubicación actual del usuario
- Uso de coordenadas para mostrar puntos en el mapa

---

### Apertura de Enlaces
- Redirección a sitios web desde la aplicación
- Uso de navegador externo mediante URL Launcher

---

### Persistencia de Datos
- Uso de base de datos local (SQLite) para almacenamiento de información
- Registro de lecturas realizadas

---

### Gestión de Lecturas
- Eliminación de lecturas desde la aplicación
- Envío de lecturas eliminadas a una API REST
- Asociación de datos al usuario autenticado

---

### Consulta de Datos
- Visualización de lecturas almacenadas en base de datos

---

## Tecnologías Utilizadas

- **Framework**: Flutter  
- **Lenguaje**: Dart  
- **Base de Datos Local**: SQLite (sqflite)  
- **Mapas**: Google Maps (google_maps_flutter)  
- **Geolocalización**: geolocator  
- **Lectura de QR**: (implementado en clase)  
- **Apertura de URLs**: url_launcher  
- **Consumo de API**: REST  

---

## Limitaciones del Proyecto
Debido al alcance del desarrollo, no se logró implementar completamente:

- Trazado de rutas desde la ubicación actual del usuario hasta el punto del QR  
- Actualmente solo se muestra la ubicación del destino en el mapa  

Esta funcionalidad queda como mejora futura del sistema.

---

## Flujo de Uso
1. El usuario inicia sesión en la aplicación  
2. Escanea un código QR  
3. La app interpreta el contenido del QR:
   - Si es geográfico → muestra ubicación en el mapa  
   - Si es URL → abre enlace externo  
4. Se registra la lectura en la aplicación  
5. El usuario puede consultar o eliminar lecturas  

---

## Ejemplos de QR Utilizados
- QR con coordenadas geográficas (ubicación en Cali)
- QR con enlace web (ej: Wikipedia)

---

## Posibles Mejoras
- Implementación de rutas en tiempo real (Google Directions API)
- Integración con backend completo para historial de usuario
- Mejora de interfaz de usuario (UX/UI)
- Implementación de recomendaciones turísticas
- Soporte offline para mapas

---

## Integrantes del Proyecto

- Lina María Fernández García  
- Joan Sebastián Tunubala Sánchez  
- Gissel Vanessa Quitian

---

## Conclusión
Este proyecto permitió integrar múltiples capacidades del desarrollo móvil en Flutter, combinando geolocalización, manejo de datos y consumo de servicios externos.

Además, representa una solución aplicable a contextos reales como el turismo inteligente, donde la tecnología mejora la interacción del usuario con el entorno.

---