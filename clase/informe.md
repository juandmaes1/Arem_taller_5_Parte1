#  Informe Técnico del Taller

##  Nombre del Taller  
**Taller 5 - Evaluación de Seguridad con STRIDE**

---

##  Integrantes del equipo  
- David Santiago Medina (davidmebu@unisabana.edu.co)
- Santiago Navarro (santiagonacu@unisabana.edu.co)
- Jacobo Pacheco (jacobopama@unisabana.edu.co)
- Juan Diego Martínez (juandmaes@unisabana.edu.co)

---

##  Descripción general del trabajo  

El objetivo de este taller fue identificar y analizar riesgos de seguridad en un sistema utilizando el marco STRIDE, el cual permite clasificar amenazas en seis categorías: Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service y Elevation of Privilege.  

Para el desarrollo de la actividad, se seleccionó como caso base la plataforma EdukIT, enfocándose en un flujo crítico del sistema: el proceso de autenticación y acceso de estudiantes a los cursos. A partir de este flujo, se identificaron vulnerabilidades, escenarios de ataque, impactos y posibles estrategias de mitigación, consolidando la información en una tabla estructurada.

---

##  Proceso de desarrollo  

Inicialmente, el equipo analizó el contexto del sistema EdukIT y seleccionó el flujo de autenticación debido a su criticidad en el control de acceso a la información. Posteriormente, se descompuso el flujo en sus componentes principales, como el módulo de autenticación, gestión de sesiones, APIs y control de acceso.  

Se aplicó el modelo STRIDE identificando amenazas específicas para cada componente. Luego, se evaluaron los posibles impactos y probabilidades, asignando un nivel de riesgo a cada amenaza. Finalmente, se definieron controles existentes y se propusieron medidas de mitigación alineadas con buenas prácticas de ciberseguridad, como autenticación multifactor (MFA), cifrado de datos y control de acceso basado en roles (RBAC).  

La herramienta principal utilizada fue Microsoft Excel para estructurar la tabla de análisis, permitiendo una visualización clara de los riesgos.

---

##  Análisis del modelo propuesto  

El modelo propuesto se estructura a partir de una tabla que organiza las amenazas según las categorías del marco STRIDE, vinculándolas con los componentes del sistema y los activos afectados. Esto permite una visión integral de los riesgos de seguridad en el flujo analizado.  

El modelo representa adecuadamente las necesidades del cliente, ya que identifica riesgos sobre información sensible como credenciales, datos personales y control de acceso. Además, permite priorizar amenazas según su impacto en la confidencialidad, integridad y disponibilidad del sistema.  

Se asumió que el sistema EdukIT cuenta con una arquitectura web estándar con autenticación basada en credenciales, uso de APIs y gestión de sesiones mediante cookies. También se consideró que existen controles básicos de seguridad, pero no mecanismos avanzados como autenticación multifactor o protección robusta contra ataques.

---

## 📈 Diagrama final entregado  

El análisis del sistema se presenta en la tabla STRIDE desarrollada en el siguiente archivo:

📁 `clase/tabla-stride-clase.xlsx`

---

##  Tabla de actores, entidades o componentes  

| Nombre del elemento | Tipo | Descripción | Responsable |
|--------------------|------|------------|-------------|
| Estudiante | Actor | Usuario que accede a cursos y contenido educativo | Usuario |
| Módulo de Autenticación | Componente | Valida credenciales de acceso | Backend |
| Gestión de Sesiones | Componente | Administra sesiones activas del usuario | Backend |
| API de Usuario | Componente | Maneja datos personales y académicos | Backend |
| Control de Acceso | Componente | Define roles y permisos del sistema | Backend |

---

##  Investigación complementaria  

**Tema investigado:** Principios de seguridad STRIDE  

**Resumen:**  

El modelo STRIDE, propuesto por Microsoft, es una metodología utilizada para identificar amenazas de seguridad en sistemas de software. Clasifica los riesgos en seis categorías: Spoofing (suplantación), Tampering (manipulación), Repudiation (repudio), Information Disclosure (divulgación de información), Denial of Service (denegación de servicio) y Elevation of Privilege (escalamiento de privilegios). Este enfoque permite analizar vulnerabilidades desde diferentes perspectivas y diseñar controles adecuados.  

En el contexto del taller, STRIDE permitió identificar riesgos críticos en el proceso de autenticación de EdukIT, destacando amenazas como el robo de credenciales, la manipulación de sesiones y el acceso indebido a información sensible. La aplicación de este modelo facilita la toma de decisiones en seguridad y contribuye a mejorar la protección de los sistemas.  

---

##  Referencias  

[1] Microsoft. *The STRIDE Threat Model*. https://learn.microsoft.com  
[2] OWASP Foundation. *OWASP Top 10*. https://owasp.org  
[3] NIST. *Cybersecurity Framework*. https://www.nist.gov  

---

Este documento hace parte de la entrega del Taller 5 del curso AREM (Arquitectura Empresarial) - Universidad de La Sabana.
