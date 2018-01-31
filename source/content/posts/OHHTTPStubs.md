---
title: "Usando OHHTTPStubs en nuestros proyectos"
date: 2018-01-31T19:36:21Z
draft: true
---

Teniendo los conceptos sobre [stubs y mocks](/posts/stubs), ahora vamos a un ejemplo real:

# Usando OHHTTPStubs

[OHHTTPStubs](https://github.com/AliSoftware/OHHTTPStubs) es una librería que nos facilita la implementación de stubs,
en este caso lo aplicamos en nuestras pruebas unitarias.

# Instalación de la librería

Existen varios medios para instalar la librería, en este post se usará mediante [cocoapods]()

# Ejemplos de OHHTTPStubs

Creamos un archivo con extensión **.swift** donde colocaremos las funciones **stub**:

[printscreen en donde es creado y ubicado el archivo]

## Simulando el método GET

Definimos la función **getRemoteInfoSuccess**