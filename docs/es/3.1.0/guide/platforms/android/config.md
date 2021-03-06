---
license: >
    Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
    with the License.  You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing,
    software distributed under the License is distributed on an
    "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
---

# Configuración de Android

El archivo `config.xml` controla la configuración básica de una app que se aplican a través de cada aplicación y una instancia de CordovaWebView. Esta sección detalla las preferencias que se aplican sólo a estructuras Android. Vea el archivo config.xml archivo para obtener información sobre las opciones de configuración global.

*   `KeepRunning` (por defecto valor booleano, `true`): determina si la aplicación queda funcionando en segundo plano, incluso después de un `pause` de evento se desencadena.
    
        <preference name="KeepRunning" value="false"/>
        

*   `ErrorUrl`: especifica una página de error que aparece en respuesta a los errores estándar HTTP en el rango de 400-500. Coloque el archivo especificado en el nivel de directorio que contiene la página de inicio y otros activos de la web.
    
        <preference name="ErrorUrl" value="error.html"/>
        

*   `LoadingDialog`: muestra un diálogo nativo cuando se carga la aplicación. El formato del valor es *título, mensaje*
    
        <preference name="LoadingDialog" value="Please wait, the app is loading"/>
        

*   `LoadingPageDialog`: muestra un diálogo nativo al cargar subpáginas dentro de una aplicación. El formato del valor es *título, mensaje*
    
        <preference name="LoadingPageDialog" value="Please wait, the data is loading"/>
        

*   `LoadUrlTimeoutValue` (número, el valor predeterminado es `20000`): cuando se carga una página, la cantidad de tiempo de espera antes de tirar un error de tiempo de espera. Este ejemplo especifica 10 segundos en lugar de 20:
    
        <preference name="LoadUrlTimeoutValue" value="10000"/>
        

*   `SplashScreen`: el nombre del archivo sin su extensión en el directorio `res/drawable`. Varios activos deben compartir este nombre común en diferentes subdirectorios.
    
        <preference name="SplashScreen" value="splash"/>
        

*   `SplashScreenDelay` (número, el valor predeterminado de `5000`): la cantidad de tiempo que muestra la imagen en pantalla splash.
    
        <preference name="SplashScreenDelay" value="10000"/>