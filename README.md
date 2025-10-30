# Assitence
# Sistema de Asistencia por Reconocimiento Facial (UNEMI)

Este proyecto es un aplicativo web desarrollado en Python y Django como parte de la Práctica #3 de la asignatura "Construcción de Software". El sistema implementa un control de asistencia en tiempo real utilizando OpenCV y la biblioteca `face_recognition` para validar la identidad de un usuario logueado contra su foto de perfil registrada.

El objetivo principal es cumplir con la guía de práctica: "Diseñar y desarrollar un aplicativo web en Django que capture imágenes o video en tiempo real, los procese con OpenCV, detecte o reconozca elementos específicos y muestre resultados útiles al usuario...".

## Contexto Académico

* **Universidad:** Universidad Estatal de Milagro (UNEMI) 
* **Facultad:** Facultad Ciencias E Ingeniería
* **Carrera:** Software 
* **Asignatura:** Construcción de Software 
* **Docente de Práctica:** Ing. Almache Sanisaca Mariana Madeleine 

## Características Principales

* **Autenticación de Usuarios:** Sistema completo de registro, inicio de sesión y cierre de sesión de Django.
* **Perfiles de Usuario:** Cada usuario tiene un perfil donde puede cargar su foto de referencia para el reconocimiento.
* **Streaming en Tiempo Real:** Transmisión de video desde la cámara web al navegador usando `StreamingHttpResponse` de Django y OpenCV.
* **Reconocimiento Facial:** El sistema no solo detecta rostros, sino que **reconoce** si el rostro en el video pertenece al usuario que ha iniciado sesión, comparándolo con su foto de perfil.
* **Prueba de Vida (Liveness Check):** Para evitar el uso de fotos, el usuario debe realizar una simple prueba de "mover el rostro" y "quedarse quieto" para validar la asistencia.
* **Registro de Asistencia:** Una vez validado, el sistema guarda automáticamente un registro de asistencia en la base de datos con el usuario y la fecha/hora.
* **Dashboard Interactivo:** La interfaz, construida con Bootstrap, muestra el conteo de rostros y el estado del sistema en tiempo real (ej. "Buscando...", "Mueve tu rostro", "Asistencia Registrada").
* **Notificaciones:** Se utiliza SweetAlert2 para mostrar un popup "hermoso" y funcional al momento de confirmar la asistencia.

## Tecnologías Utilizadas

### Backend
* **Python 3.x** 
* **Django** (Framework Web) 
* **OpenCV** (Para captura de video y procesamiento de imagen)
* **face_recognition** (Para el reconocimiento facial y comparación)
* **dlib** (Dependencia de `face_recognition`)
* **Numpy** (Para operaciones de imagen)

### Frontend
* **HTML5**
* **Bootstrap 5**
* **JavaScript (ES6+)**
* **SweetAlert2** (Para notificaciones)

## Instalación y Puesta en Marcha

Sigue estos pasos para ejecutar el proyecto en tu máquina local.

**1. Clonar el Repositorio**

git clone [[https://github.com/tu-usuario/tu-repositorio.git](https://github.com/ofdaniOnfire/Assitence.git)]
cd repositorio
