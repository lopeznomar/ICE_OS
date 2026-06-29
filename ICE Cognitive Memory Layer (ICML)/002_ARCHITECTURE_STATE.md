\# 002\_ARCHITECTURE\_STATE.md



\# ICE™ ARCHITECTURE STATE



\*\*Estado Oficial de la Arquitectura del Proyecto\*\*



\*\*Versión:\*\* 1.0

\*\*Estado:\*\* Arquitectura Base Aprobada



\---



\# Objetivo



Este documento describe la arquitectura funcional y técnica vigente de ICE™.



Su propósito es proporcionar una visión clara de cómo está organizado el sistema y servir como referencia para cualquier desarrollo futuro.



Toda modificación arquitectónica deberá reflejarse en este documento.



\---



\# Principio Arquitectónico



ICE™ no es un ERP.



ICE™ es una plataforma de Inteligencia Ejecutiva que consume información proveniente de uno o varios ERP para transformarla en conocimiento útil para la dirección de la empresa.



El ERP continúa siendo el sistema transaccional.



ICE™ actúa como una capa superior de análisis e inteligencia.



\---



\# Arquitectura General



```text

&#x20;                  Empresario

&#x20;                       │

&#x20;                       ▼

&#x20;            Landing ICE™ / Website

&#x20;                       │

&#x20;                       ▼

&#x20;               ICE Beacon

&#x20;                       │

&#x20;                       ▼

&#x20;           Executive Assessment

&#x20;                       │

&#x20;                       ▼

&#x20;                ICE Score™

&#x20;                       │

&#x20;                       ▼

&#x20;           Executive Report™

&#x20;                       │

&#x20;                       ▼

&#x20;            Plataforma ICE™

&#x20;                       │

&#x20;       ┌───────────────┼───────────────┐

&#x20;       ▼               ▼               ▼

&#x20;    Dashboard       IA Generativa   Reglas de Negocio

&#x20;       │               │               │

&#x20;       └───────────────┼───────────────┘

&#x20;                       ▼

&#x20;                 API de Integración

&#x20;                       │

&#x20;       ┌───────────────┼───────────────┐

&#x20;       ▼               ▼               ▼

&#x20;     SAINT         Otros ERP       Fuentes Externas

```



\---



\# Capas del Sistema



\## 1. Capa de Presentación



Es el punto de contacto con el usuario.



Incluye:



\* Landing pública.

\* Sitio institucional.

\* Formularios.

\* ICE Beacon.

\* Executive Assessment.

\* Portal del cliente.



Objetivo:



Generar una experiencia clara, profesional y orientada al empresario.



\---



\## 2. Capa de Experiencia



Aquí ocurre la interacción inteligente.



Componentes:



\* ICE Beacon.

\* Executive Assessment.

\* Executive Score.

\* Executive Report.



Esta capa transforma la navegación en una conversación.



\---



\## 3. Capa de Inteligencia



Es el núcleo del sistema.



Responsabilidades:



\* interpretación de indicadores;

\* generación de recomendaciones;

\* análisis ejecutivo;

\* detección de riesgos;

\* priorización de problemas.



Aquí reside el verdadero valor de ICE™.



\---



\## 4. Capa de Negocio



Contiene las reglas funcionales del producto.



Ejemplos:



\* cálculo de indicadores;

\* clasificación de riesgos;

\* evaluación financiera;

\* interpretación operacional;

\* generación de alertas.



Estas reglas representan el conocimiento acumulado del fundador.



\---



\## 5. Capa de Integración



Responsable de comunicarse con sistemas externos.



Inicialmente:



\* SAINT ERP.



Posteriormente:



\* SAP.

\* Odoo.

\* Microsoft Dynamics.

\* Oracle.

\* Zoho.

\* QuickBooks.

\* otros ERP.



La arquitectura debe ser desacoplada.



\---



\## 6. Capa de Datos



Administra la información utilizada por ICE™.



Incluye:



\* indicadores;

\* configuraciones;

\* resultados de evaluaciones;

\* historial;

\* métricas;

\* modelos de IA.



\---



\# Componentes Principales



\## Landing



Objetivo:



Presentar la propuesta de valor de ICE™ y conducir al visitante hacia el Executive Assessment.



Estado:



En evolución.



\---



\## ICE Beacon



Primer contacto inteligente con el empresario.



No debe comportarse como publicidad.



Debe iniciar una conversación.



Estado:



En desarrollo.



\---



\## Executive Assessment



Cuestionario ejecutivo diseñado para identificar oportunidades y riesgos.



Resultado:



Executive Score.



Estado:



Diseño funcional aprobado.



\---



\## Executive Score™



Resultado cuantitativo de la evaluación.



Debe ser:



\* claro;

\* visual;

\* accionable.



Estado:



Pendiente.



\---



\## Executive Report™



Informe ejecutivo generado automáticamente.



Debe contener:



\* fortalezas;

\* debilidades;

\* riesgos;

\* oportunidades;

\* prioridades.



Estado:



Pendiente.



\---



\## Dashboard Ejecutivo



Permitirá visualizar la situación general de la empresa.



No reemplaza reportes tradicionales.



Resume únicamente la información necesaria para decidir.



Estado:



Pendiente.



\---



\# Integración con SAINT ERP



Primera etapa del proyecto.



Objetivos:



\* lectura segura de información;

\* extracción de indicadores;

\* mínima intervención sobre el ERP;

\* independencia tecnológica.



ICE™ no modificará la lógica interna de SAINT.



Consumirá información y generará inteligencia.



\---



\# Tecnologías Objetivo



Frontend



\* HTML5

\* CSS3

\* JavaScript

\* React (cuando sea necesario)



Backend



\* Python

\* FastAPI



Base de datos



\* SQL Server

\* PostgreSQL (evaluación futura)



Servicios IA



\* OpenAI

\* Modelos futuros compatibles



Repositorio



\* GitHub



Despliegue



\* Netlify (Landing)

\* Infraestructura Cloud para la plataforma.



\---



\# Principios de Desarrollo



Toda nueva funcionalidad deberá cumplir:



\* modularidad;

\* bajo acoplamiento;

\* alta cohesión;

\* facilidad de mantenimiento;

\* escalabilidad;

\* simplicidad.



\---



\# Estado Actual de la Arquitectura



| Componente           | Estado          |

| -------------------- | --------------- |

| Landing              | Activa          |

| GitHub               | Activo          |

| Documentación        | En crecimiento  |

| ICE Beacon           | En construcción |

| Executive Assessment | Diseño aprobado |

| Executive Score      | Pendiente       |

| Executive Report     | Pendiente       |

| Dashboard            | Pendiente       |

| API                  | Pendiente       |

| Integración SAINT    | Planificada     |



\---



\# Próxima Evolución Arquitectónica



La siguiente fase consistirá en construir completamente el flujo:



Landing



↓



ICE Beacon



↓



Executive Assessment



↓



Executive Score



↓



Executive Report



Este flujo constituye el Producto Mínimo Viable (MVP) de ICE™.



\---



\# Regla Arquitectónica Fundamental



Toda decisión técnica deberá responder a la siguiente pregunta:



> \*\*¿Esta arquitectura facilita que un empresario tome mejores decisiones?\*\*



Si la respuesta es negativa, deberá replantearse la implementación.



\---



\# Documento Vivo



Este documento deberá actualizarse cuando exista un cambio significativo en la arquitectura, incorporación de nuevos componentes o modificación del flujo principal del producto.



\---



\# Fin del documento



