# Readme Grupo 4
## Introducción
Trivy es una herramienta que permite escánear vulnerabilidades de codigo de imagenes contenedoras.

###INTEGRANTES:
- Carlos Chicaiza
- Jessica Llumiguano
- Emilio Mayorga
- Juan Vizuete

## Descripcion
Trivy es un escáner de seguridad integral y versátil desarrollado por Aqua Security. Está diseñado para identificar vulnerabilidades y problemas de configuración en una amplia gama de objetivos, incluyendo imágenes de contenedores, sistemas de archivos, repositorios de código, máquinas virtuales, clústeres de Kubernetes y entornos en la nube. 

## Funcionalidades principales

### •	Escaneo de imágenes de contenedores
Trivy analiza imágenes de contenedores en busca de vulnerabilidades conocidas en paquetes del sistema operativo y dependencias de aplicaciones. Soporta múltiples sistemas operativos y gestores de paquetes, como Alpine, RHEL, CentOS, Debian, Ubuntu, npm, yarn, entre otros. 

### •	Análisis de sistemas de archivos y repositorios de código
Permite escanear sistemas de archivos locales y repositorios de código (tanto locales como remotos) para detectar vulnerabilidades en dependencias y configuraciones. Es compatible con diversos lenguajes y entornos de desarrollo. 

### •	Detección de problemas de configuración y secretos
Identifica problemas de configuración en infraestructuras como código (IaC) y busca información sensible o secretos que puedan estar expuestos en el código o en la configuración. 

### •	Análisis de licencias de software
Trivy evalúa las licencias de las dependencias utilizadas, ayudando a garantizar el cumplimiento con las políticas de licencias y evitando posibles conflictos legales. 

### •	Operador Trivy para Kubernetes
El Trivy Operator extiende las capacidades de Trivy al entorno de Kubernetes, realizando escaneos continuos de seguridad en clústeres y generando informes detallados sobre los recursos y configuraciones.  

## Justificación Técnica

### 1. Escaneo Rápido
Trivy es conocido por su velocidad y precisión en la detección de vulnerabilidades, minimizando los falsos positivos que pueden afectar la confianza de los usuarios en las herramientas de seguridad

### 2. Actualizaciones continuas de la DB
Trivy actualiza regularmente su base de datos de vulnerabilidades lo que proporciona información de seguridad más reciente para un escaneo mas efectivo. Esto es crucial para identificar y mitigar amenzas emergentes de manera proactiva.

### 3. Soporte multientono
Es versatil y puede escanear contenedores, sistemas de archivos, repositorios de código y configuraciones de infraestructura. Esta versatilidad permite una detección exhaustiva de vulnerabilidades en múltiples componenetes del entorno de desarrollo y producción

### 4. Integración CI/CD

Está diseñado teniendo en cuenta la automatización, trivy integra sin problemas en las canalización de CI/CD, lo que permite comprobaciones de seguridad en los flujos de trabajo de desarrollo. Además, su rapidez en el escaneo permite integrarlo eficientemente en las canalizaciones de CI/CD sin compormeter los tiempos de entrega.


## Características destacadas (Justificación Técnica)

### 1. Cobertura Integral
Trivy detecta vulnerabilidades en:
- Paquetes de sistemas operativos (Alpine, RHEL, CentOS, etc.).
- Dependencias de aplicaciones gestionadas por Bundler, Composer, npm, yarn, entre otros.
- Configuraciones incorrectas en Kubernetes y archivos IaC (Infrastructure as Code).

### 2. Integración en CI/CD
Trivy se integra fácilmente en pipelines de Integración Continua y Entrega Continua (CI/CD), facilitando la detección temprana de vulnerabilidades durante el ciclo de desarrollo del software.

### 3. Simplicidad y Rapidez
La herramienta destaca por su facilidad de uso y velocidad en el escaneo, permitiendo a los desarrolladores y equipos de seguridad identificar vulnerabilidades sin complicaciones.

### 4. Comunidad Activa y Soporte
Al ser un proyecto de código abierto respaldado por [Aqua Security](https://www.aquasec.com/), Trivy cuenta con una comunidad activa que contribuye a su mejora continua y ofrece soporte a los usuarios.

### 5. Escaneo de imágenes de contenedores
Detecta vulnerabilidades en paquetes del sistema operativo y bibliotecas incluidas en las imágenes de contenedores.

### 6. Análisis de dependencias
Examina las dependencias de proyectos en lenguajes como Ruby, JavaScript y Python en busca de vulnerabilidades conocidas.


Trivy es ideal para equipos de desarrollo y operaciones que utilizan tecnologías de contenedores y desean garantizar que sus imágenes y dependencias estén libres de vulnerabilidades antes de su implementación.

  
### Complementos útiles: Autoruns y TCPView

Aunque Trivy es la mejor opción para analizar seguridad en contenedores y aplicaciones modernas, existen otras herramientas que pueden complementar su uso cuando trabajamos con sistemas Windows tradicionales o queremos monitorear procesos y conexiones en ejecución.
  
#### Autoruns: Control sobre procesos de inicio en Windows

¿Para qué sirve?
Autoruns permite ver qué programas se inician automáticamente en Windows, ayudando a identificar posibles software malicioso o procesos no deseados que podrían afectar la seguridad del sistema.

Casos de uso complementarios a Trivy:
Si un ataque compromete un servidor Windows, Autoruns ayuda a identificar procesos sospechosos.
Se usa para eliminar malware persistente que se inicia automáticamente.


#### TCPView: Monitoreo de conexiones de red en tiempo real

¿Para qué sirve?
TCPView permite ver en tiempo real todas las conexiones de red activas en un sistema Windows, facilitando la detección de conexiones sospechosas o tráfico malicioso.

Casos de uso complementarios a Trivy:
Si Trivy detecta vulnerabilidades en un sistema, TCPView ayuda a ver si hay conexiones sospechosas activas.
Es útil para analizar ataques en curso o detectar malware que comunique con servidores externos.

### Complementando con Autoruns y TCPView:
Si bien Trivy es ideal para escaneo de vulnerabilidades en contenedores y código, herramientas como Autoruns y TCPView pueden ser útiles en seguridad de sistemas Windows, permitiendo monitorear procesos sospechosos y conexiones de red en tiempo real.


Hemos escogido a Trivy como la herramienta principal para el análisis de seguridad debido a su enfoque integral en la detección de vulnerabilidades en contenedores, imágenes de Docker, infraestructura como código (IaC) y dependencias de software. En un entorno donde la seguridad en la nube y la automatización de DevSecOps son fundamentales, Trivy se posiciona como una solución eficiente, rápida y altamente adaptable a los flujos de trabajo modernos.

Además, su compatibilidad con SBOM (Software Bill of Materials) y su capacidad para identificar fallos en configuraciones de seguridad en Kubernetes, Terraform y Docker lo convierten en la mejor opción para evaluar la postura de seguridad en entornos cloud-native.

En comparación con herramientas como Autoruns y TCPView, que están diseñadas para auditorías en sistemas Windows y análisis de tráfico de red respectivamente, Trivy ofrece una solución más amplia y automatizada, alineándose con los estándares actuales de seguridad en la nube y el ciclo de desarrollo seguro.

Por estas razones, el Grupo 4 ha optado por Trivy como la herramienta principal, complementándola con otras soluciones cuando sea necesario para análisis específicos en entornos locales o sistemas operativos tradicionales.

## Conclusión

Trivy es la mejor opción para análisis de vulnerabilidades en entornos modernos como Kubernetes, Docker y CI/CD, proporcionando detección proactiva y automatizada de riesgos de seguridad.

Autoruns y TCPView pueden ser herramientas complementarias en auditorías de seguridad en Windows, pero no reemplazan la capacidad de análisis de Trivy en contenedores y código.

## Recomendación
Si el entorno de seguridad se enfoca en infraestructura en la nube y DevSecOps, Trivy es la herramienta principal a utilizar. En cambio, si el análisis se realiza en endpoints Windows o redes corporativas, Autoruns y TCPView pueden ser útiles como herramientas secundarias.


## Referencias
- CloudThat. (2024). Detecting and Fixing Vulnerabilities in Docker Images with Trivy and Best Practices. Recuperado de https://www.cloudthat.com/resources/blog/detecting-and-fixing-vulnerabilities-in-docker-images-with-trivy-and-best-practices
- Trivy. Ecosystem. Recuperado de https://trivy.dev/v0.59/ecosystem/
- Aqua. (2021). Trivy´s Journey: From personal project to Open Source Scanner of Choice. Recuperado de https://www.aquasec.com/blog/trivy-scanner/
- Medium. (2024). Catching Vulnerabilities in Your Docker Images: The Power of trivy. Recuperado de https://medium.com/%40sachinsoni600517/catching-vulnerabilities-in-your-docker-images-the-power-of-trivy-6c86494b0564
- Análisis de contenedores utilizando TRIVY – IberAsync.es - https://iberasync.es/analisis-de-contenedores-utilizando-trivy/
- Container vulnerability scanning with Trivy – Bluetab - https://www.bluetab.net/en/container-vulnerability-scanning-with-trivy/
- Guía de Autoruns en Microsoft Learn - https://learn.microsoft.com/en-us/sysinternals/downloads/autoruns
- Aquasecurity. Trivy. Recuperado de https://github.com/aquasecurity/trivy
- Trivy. Repositorio de codigo. Recuperado de https: https://trivy.dev/latest/docs/target/repository/

