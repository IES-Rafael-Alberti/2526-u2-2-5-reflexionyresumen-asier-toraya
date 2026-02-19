# RESPUESTAS - Reflexión y Resumen

> **Actividad / ID:** 2526-u2-2-5
> **Unidad / Tema:** Unidad 2 - Detección, clasificación y gestión de incidentes.
> **Alumno/a:** Asier Toraya
> **Fecha:** 23/02/2026

---

## 1) Reflexión crítica (preguntas)

### 1.1) ¿Qué te han parecido los temas tratados en la unidad?

La unidad está bien organizada porque conecta todo el ciclo de trabajo real en un equipo defensivo: clasificar, detectar, investigar, responder y dejar trazabilidad. Además no solo es teórico sino que entra en temas operativos, fases de implementación del SIEM, priorización peligrosidad/impacto...
A nivel técnico, la mayor aportación es entender que la seguridad no depende de una herramienta aislada, sino de la integración personas + procesos + tecnología + evidencia documental.

### 1.2) ¿Qué ha sido más útil para tu futuro puesto de trabajo? ¿Por qué?

Lo más útil para un puesto SOC es la combinación de la priorización de incidentes con taxonomía + impacto + peligrosidad.
Ver el flujo SIEM -> IMS -> playbook -> cierre, también considero que es útil. El tema de la documentación estructurada para mejorar reglas y justificar decisiones me parece muy importante porque sin todo esto puede llegar a convertir la investigación en inconsistente y llevar a la pérdida de conocimiento operativo.

### 1.3) ¿Qué partes ya conocías y cuáles han sido nuevas para ti?

Tenía ideas generales de OSINT pero me ha gustado mucho todo lo que hemos visto que me ha permitido aumentar mis conocimientos sobre esta materia.
He aprendido el funcionamiento básico del SIEM y a documentar de una forma más estructurada. También sobre la taxonomía de incidentes y la matriz de prioridad.

### 1.4) ¿Qué concepto/idea te ha llamado más la atención y por qué?

Me ha llamado especialmente la diferencia entre peligrosidad e impacto, ya que cambia totalmente la toma de decisiones a la hora de afrontar una incidencia. Debido a que un ataque técnicamente sofisticado puede tener poco impacto pero uno simple puede generar un impacto crítico por falta de resiliencia.

Esta diferencia evita errores de gestión como sobrerreaccionar a técnica "llamativa" o infravalorar incidentes "simples" con alto daño operativo.

### 1.5) ¿Qué parte recortarías o simplificarías si hubiera menos tiempo? Justifica.

La verdad que en esta unidad hay pocas cosas que recortar porque todo es necesario, tal vez recortaría parte del bloque histórico o de enumeración extensa de herramientas concretas y concentraría más tiempo en laboratorios guiados como la práctica del SIEM, ya que para puestos SOC juniors interesa más practicar triage de alertas, ajuste de reglas y redacción de informes con evidencia.

### 1.6) ¿Qué tema has echado en falta o ampliarías? Justifica.

Ampliaría el contenido con más prácticas del SIEM como casos reales de reducción de falsos positivos, automatización SOAR, backlogs... Creo que son temas clave para medir madurez y no quedarse sin afianzar bien la teoría.

### 1.7) ¿Qué aplicarías "mañana" en un entorno real con recursos limitados?

Aplicaría un mínimo viable de operación:

* Inventario de fuentes de log críticas (AD, firewall, endpoint, correo).
* Casos de uso SIEM (phishing, brute force, exfiltración básica...)
* Playbooks cortos de triage (quién, qué revisar...).
* Plantilla única de incidente (datos generales, clasificación, IOC, timeline, acciones...).
* Revisión semanal de alertas falsas y ajuste de reglas.

Con poco equipo y recursos se puede mejorar consistencia, trazabilidad y tiempo de respuesta.

### 1.8) ¿Qué duda, riesgo o punto crítico te queda abierto tras la unidad?

La duda que más me queda es hasta qué punto conviene automatizar respuestas en SOAR sin pasarse, porque si se bloquea algo de forma automática sin tener suficiente contexto se puede cortar un servicio legítimo o incluso perder evidencia importante. Por eso, ahora mismo lo veo más seguro para un entorno real automatizar solo tareas de bajo riesgo y dejar con validación humana las acciones que sean irreversibles.

## 2) Resumen esquematizado (obligatorio)

### 2.1) Mapa/índice de la unidad (visión global)

- **Bloque A - Fundamentos y clasificación**
  - Categorías de seguridad SI (ENS): niveles BAJO/MEDIO/ALTO; categoría BÁSICA/MEDIA/ALTA.
  - Taxonomía de incidentes: tipos, factores de clasificación, peligrosidad, impacto, prioridad y respuesta.
- **Bloque B - Detección y operación SOC**
  - Indicios: precursores e indicadores.
  - SOC: objetivos, roles, procesos, servicios, tecnologías, modelos organizativos.
  - Diferencias SOC vs CERT/CIRT/CSIRT.
  - IDS/IPS/SIEM e IoC.
- **Bloque C - SIEM y casos de uso**
  - SIEM: logs, recolección, agregación, EPS, enriquecimiento, almacenamiento, alerting.
  - Gestión de incidentes (IMS), naming de casos, playbooks, flujo de analista.
  - Casos de uso SOC: creación, validación y mejora continua.
  - Marco MaGMa: negocio, amenaza, implementación.
- **Bloque D - Implantación y evolución**
  - Fases SIEM: descubrimiento/planificación -> piloto -> implantación -> mejora continua.
  - Mejores prácticas: objetivos claros, casos de uso, runbooks, iteración.
  - Evolución SIEM + SOAR: orquestación, automatización, respuesta.
- **Bloque E - OSINT**
  - Conceptos, ciclo OSINT (6 fases), técnicas, herramientas y casos prácticos.
  - Límites legales/éticos (privacidad y normativa).
- **Bloque F - Documentación e informe técnico**
  - Qué documentar en un incidente, seguimiento, cierre y lecciones aprendidas.
  - Cómo redactar informes técnicos claros, accionables y adaptados a audiencia.

### 2.2) Conceptos clave (lista breve)

- Categorización ENS.
- Incidente vs incidencia.
- Taxonomía de incidentes (contenido abusivo/malicioso, obtención información, intento intrusión, intrusión, disponibilidad, compromiso información, fraude, vulnerable, otros).
- Peligrosidad, impacto, prioridad.
- Precursor vs indicador.
- IoC e IoA.
- SOC (N1/N2/N3), threat intelligence, threat hunting, forense, purple team.
- IDS, IPS, SIEM, SOAR.
- EPS, parsing, enriquecimiento, WORM, blacklist/whitelist/long tail.
- IMS, ticket/caso, playbook, verdadero positivo/falso positivo.
- Caso de uso SOC.
- OSINT, footprinting/fingerprinting.
- Timeline, runbook, post-mortem, lecciones aprendidas.

### 2.3) Procesos / procedimientos (pasos o checklist)

- **Proceso de gestión de incidentes (macro)**
  - 1. Preparación.
  - 2. Identificación.
  - 3. Contención.
  - 4. Erradicación.
  - 5. Recuperación.
  - 6. Lecciones aprendidas.
- **Proceso de clasificación y priorización**
  - 1. Tipificar incidente (taxonomía).
  - 2. Estimar peligrosidad.
  - 3. Estimar impacto.
  - 4. Asignar prioridad y SLA.
  - 5. Ejecutar respuesta acorde.
- **Proceso operativo SIEM/IMS**
  - 1. Ingesta de logs (agente/syslog/agentless).
  - 2. Normalización + enriquecimiento.
  - 3. Correlación y alerta.
  - 4. Creación de caso en IMS.
  - 5. Triage con playbook.
  - 6. Cierre (TP/FP) + feedback a reglas.
- **Proceso OSINT**
  - 1. Planificación.
  - 2. Identificación de fuentes.
  - 3. Adquisición.
  - 4. Procesamiento.
  - 5. Análisis.
  - 6. Difusión/inteligencia.
- **Checklist mínimo de documentación de incidente**
  - Datos generales (quién, cuándo, cómo se detectó).
  - Clasificación y valoración.
  - IOCs/TTPs y activos afectados.
  - Acciones realizadas + timeline.
  - Impacto y consecuencias.
  - Recomendaciones y plan de mejora.

### 2.4) Herramientas / tecnicas (si aplica)

- **Detección y operación**
  - SIEM (Elastic, Sentinel, QRadar, Splunk).
  - IDS/IPS (Snort).
  - EDR/NDR.
  - Ticketing/IMS (TheHive y similares).
  - SOAR (automatización/orquestación).
- **Threat intelligence / IoC**
  - STIX/TAXII, OpenIOC, IODEF, MISP (referenciado en unidad).
- **OSINT**
  - Google Dorking, WHOIS, DNS, Wayback.
  - Shodan, Maltego, SpiderFoot, Sherlock, OSINT Framework.
  - ExifTool / análisis de metadatos.
- **Técnicas destacadas**
  - Correlación de eventos.
  - Enriquecimiento de logs.
  - Búsqueda inversa de imagen.
  - Análisis de patrones de comportamiento.

### 2.5) Buenas practicas y errores tipicos

- **Buenas prácticas**
  - Definir objetivos y alcance antes de desplegar SIEM.
  - Empezar con piloto representativo y casos de uso de alto impacto.
  - Mantener playbooks y runbooks versionados.
  - Separar hechos de hipótesis en informes.
  - Registrar acciones con fecha/hora y evidencias.
  - Revisar semanalmente falsos positivos y ajustar detección.
  - Aplicar mejora continua (técnica + proceso + personas).
  - Usar OSINT con trazabilidad y dentro de legalidad.
- **Errores típicos**
  - Querer ingestar "todo" sin priorizar.
  - Confundir volumen de alertas con efectividad.
  - No medir MTTD/MTTR ni calidad de detección.
  - No documentar decisiones durante el incidente.
  - Automatizar respuestas críticas sin control humano.
  - Usar OSINT sin validar fuentes ni marco legal.

### 2.6) Glosario mínimo (términos y definiciones cortas)

- **IoC:** Indicador técnico de posible compromiso (IP, hash, dominio, etc.).
- **IoA:** Indicador de comportamiento de ataque (acciones/tácticas).
- **SOC:** Centro de operaciones de seguridad.
- **SIEM:** Plataforma de gestión/correlación de eventos de seguridad.
- **SOAR:** Orquestación y automatización de respuesta.
- **IMS:** Sistema de gestión de incidentes/casos.
- **Playbook:** Flujo guiado de investigación/respuesta para un tipo de alerta.
- **Runbook:** Procedimiento operativo paso a paso.
- **EPS:** Eventos por segundo en ingesta de logs.
- **Triage:** Clasificación inicial de alertas para decidir prioridad/escalado.
- **TP/FP:** Verdadero positivo / falso positivo.
- **OSINT:** Inteligencia obtenida de fuentes abiertas y legales.
- **Footprinting:** Recolección de huella digital de un objetivo.
- **MITRE ATT&CK:** Marco para mapear tácticas y técnicas de adversarios.
- **MTTD/MTTR:** Tiempo medio de detección / respuesta.

## 3) (Opcional) Evidencias y recursos usados

- [Documentación de la unidad dos - https://revilofe.github.io/section2/u02/](https://revilofe.github.io/section2/u02/)

## 4) Conclusión (cierre)

En conclusión, esta unidad me ha ayudado a entender mejor cómo se trabaja un incidente de seguridad de principio a fin, no solo detectando alertas, sino también clasificando, priorizando, investigando y documentando cada paso con criterio. Me llevo como idea principal que la eficacia en ciberseguridad no depende solo de tener buenas herramientas, sino de aplicar procesos claros, mantener una buena trazabilidad y aprender de cada caso para mejorar de forma continua.
