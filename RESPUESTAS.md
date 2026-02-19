# RESPUESTAS - Reflexion y Resumen

> **Actividad / ID:** 2526-u2-2-5
> **Unidad / Tema:** Unidad 2 - Deteccion, clasificacion y gestion de incidentes (SOC, SIEM, OSINT, documentacion e informes tecnicos)
> **Alumno/a:** Asier Toraya
> **Fecha:** 18/02/2026

---

## 1) Reflexion critica (preguntas)

### 1.1) Que te han parecido los temas tratados en la unidad?

La unidad esta bien organizada porque conecta todo el ciclo de trabajo real en un equipo defensivo: clasificar, detectar, investigar, responder y dejar trazabilidad. Además no solo es teórico sino que entra en temas operativos, fases de implementacion del SIEM, priorización peligrosidad/impacto...
A nivel tecnico, la mayor aportacion es entender que la seguridad no depende de una herramienta aislada, sino de la integracion personas + procesos + tecnologia + evidencia documental.

### 1.2) Que ha sido mas util para tu futuro puesto de trabajo? Por que?

Lo mas util para un puesto SOC es la combinacion de la priorizacion de incidentes con taxonomia + impacto + peligrosidad.
Ver el flujo SIEM -> IMS -> playbook -> cierre, también considero que es útil. El tema de la documentación estructurada para mejorar relgas y justificar decisiones me parece muy importante porque sin todo esto puede llegar a convertir la investigación en inconsistente y llevar a la perdida de conocimiento operativo.

### 1.3) Que partes ya conocias y cuales han sido nuevas para ti?

Tenía ideas generales de OSINT pero me ha gustado mucho todo lo que hemos visto que me ha permitido aumentar mis conocimientos sobre esta materia.
He aprendido el funcionamiento básico del SIEM y a documentar de una forma más estructurada. También sobre la taxonomía de incidentes y la matriz de prioridad.

### 1.4) Que concepto/idea te ha llamado mas la atencion y por que?

Me ha llamado especialmente la diferencia entre peligrosidad e impacto, ya que cambia totalmente la toma de decisiones a la hora de afrontar una incidencia. Debido a que un ataque técnicamente sofisticado puede tener poco impacto pero uno simple puede generar un impacto crítico por falta de resiliencia.

Esta diferencia evita errores de gestion como sobrerreaccionar a tecnica "llamativa" o infravalorar incidentes "simples" con alto daño operativo.

### 1.5) Que parte recortarias o simplificarias si hubiera menos tiempo? Justifica.

La verdad que en esta unidad hay pocas cosas que recortar porque todo es necesario, tal vez recortaria parte del bloque historico o de enumeracion extensa de herramientas concretas y concentraria más tiempo en laboratorios guiados como la práctica del SIEM, ya que para puestos SOC juniors interesa más practicar triage de alertas, ajuste de reglas y redacción de informes con evidencia.

### 1.6) Que tema has echado en falta o ampliarias? Justifica.

Ampliaria el contenido con más prácticas del SIEM como casos reales de reduccion de falsos positivos, automatización SOAR, backlogs... Creo que son temas clave para medir madurez y no quedarse sin afianzar bien la teoria.

### 1.7) Que aplicarias "mañana" en un entorno real con recursos limitados?

Aplicaria un minimo viable de operación:

* Inventario de fuentes de log criticas (AD, firewall, endpoint, correo).
* Casos de uso SIEM (phishing, brute force, exfiltracion basica...)
* Playbooks cortos de triage (quien, que revisar...).
* Plantilla unica de incidente (datos generales, clasificacion, IOC, timeline, acciones...).
* Revision semanal de alertas falsas y ajuste de reglas.

Con poco equipo y recursos se puede mejorar consistencia, trazabilidad y tiempo de respuesta.

### 1.8) Que duda, riesgo o punto crítico te queda abierto tras la unidad?

La duda que mas me queda es hasta que punto conviene automatizar respuestas en SOAR sin pasarse, porque si se bloquea algo de forma automatica sin tener suficiente contexto se puede cortar un servicio legitimo o incluso perder evidencia importante. Por eso, ahora mismo lo veo mas seguro para un entorno real automatizar solo tareas de bajo riesgo y dejar con validacion humana las acciones que sean irreversibles.

## 2) Resumen esquematizado (obligatorio)

### 2.1) Mapa/indice de la unidad (vision global)

- **Bloque A - Fundamentos y clasificacion**
  - Categorias de seguridad SI (ENS): niveles BAJO/MEDIO/ALTO; categoria BASICA/MEDIA/ALTA.
  - Taxonomia de incidentes: tipos, factores de clasificacion, peligrosidad, impacto, prioridad y respuesta.
- **Bloque B - Deteccion y operacion SOC**
  - Indicios: precursores e indicadores.
  - SOC: objetivos, roles, procesos, servicios, tecnologias, modelos organizativos.
  - Diferencias SOC vs CERT/CIRT/CSIRT.
  - IDS/IPS/SIEM e IoC.
- **Bloque C - SIEM y casos de uso**
  - SIEM: logs, recoleccion, agregacion, EPS, enriquecimiento, almacenamiento, alerting.
  - Gestion de incidentes (IMS), naming de casos, playbooks, flujo de analista.
  - Casos de uso SOC: creacion, validacion y mejora continua.
  - Marco MaGMa: negocio, amenaza, implementacion.
- **Bloque D - Implantacion y evolucion**
  - Fases SIEM: descubrimiento/planificacion -> piloto -> implantacion -> mejora continua.
  - Mejores practicas: objetivos claros, casos de uso, runbooks, iteracion.
  - Evolucion SIEM + SOAR: orquestacion, automatizacion, respuesta.
- **Bloque E - OSINT**
  - Conceptos, ciclo OSINT (6 fases), tecnicas, herramientas y casos practicos.
  - Limites legales/eticos (privacidad y normativa).
- **Bloque F - Documentacion e informe tecnico**
  - Que documentar en un incidente, seguimiento, cierre y lecciones aprendidas.
  - Como redactar informes tecnicos claros, accionables y adaptados a audiencia.

### 2.2) Conceptos clave (lista breve)

- Categorizacion ENS.
- Incidente vs incidencia.
- Taxonomia de incidentes (contenido abusivo/malicioso, obtencion informacion, intento intrusion, intrusion, disponibilidad, compromiso informacion, fraude, vulnerable, otros).
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

- **Proceso de gestion de incidentes (macro)**
  - 1. Preparacion.
  - 2. Identificacion.
  - 3. Contencion.
  - 4. Erradicacion.
  - 5. Recuperacion.
  - 6. Lecciones aprendidas.
- **Proceso de clasificacion y priorizacion**
  - 1. Tipificar incidente (taxonomia).
  - 2. Estimar peligrosidad.
  - 3. Estimar impacto.
  - 4. Asignar prioridad y SLA.
  - 5. Ejecutar respuesta acorde.
- **Proceso operativo SIEM/IMS**
  - 1. Ingesta de logs (agente/syslog/agentless).
  - 2. Normalizacion + enriquecimiento.
  - 3. Correlacion y alerta.
  - 4. Creacion de caso en IMS.
  - 5. Triage con playbook.
  - 6. Cierre (TP/FP) + feedback a reglas.
- **Proceso OSINT**
  - 1. Planificacion.
  - 2. Identificacion de fuentes.
  - 3. Adquisicion.
  - 4. Procesamiento.
  - 5. Analisis.
  - 6. Difusion/inteligencia.
- **Checklist minimo de documentacion de incidente**
  - Datos generales (quien, cuando, como se detecto).
  - Clasificacion y valoracion.
  - IOCs/TTPs y activos afectados.
  - Acciones realizadas + timeline.
  - Impacto y consecuencias.
  - Recomendaciones y plan de mejora.

### 2.4) Herramientas / tecnicas (si aplica)

- **Deteccion y operacion**
  - SIEM (Elastic, Sentinel, QRadar, Splunk).
  - IDS/IPS (Snort).
  - EDR/NDR.
  - Ticketing/IMS (TheHive y similares).
  - SOAR (automatizacion/orquestacion).
- **Threat intelligence / IoC**
  - STIX/TAXII, OpenIOC, IODEF, MISP (referenciado en unidad).
- **OSINT**
  - Google Dorking, WHOIS, DNS, Wayback.
  - Shodan, Maltego, SpiderFoot, Sherlock, OSINT Framework.
  - ExifTool / analisis de metadatos.
- **Tecnicas destacadas**
  - Correlacion de eventos.
  - Enriquecimiento de logs.
  - Busqueda inversa de imagen.
  - Analisis de patrones de comportamiento.

### 2.5) Buenas practicas y errores tipicos

- **Buenas practicas**
  - Definir objetivos y alcance antes de desplegar SIEM.
  - Empezar con piloto representativo y casos de uso de alto impacto.
  - Mantener playbooks y runbooks versionados.
  - Separar hechos de hipotesis en informes.
  - Registrar acciones con fecha/hora y evidencias.
  - Revisar semanalmente falsos positivos y ajustar deteccion.
  - Aplicar mejora continua (tecnica + proceso + personas).
  - Usar OSINT con trazabilidad y dentro de legalidad.
- **Errores tipicos**
  - Querer ingestar "todo" sin priorizar.
  - Confundir volumen de alertas con efectividad.
  - No medir MTTD/MTTR ni calidad de deteccion.
  - No documentar decisiones durante el incidente.
  - Automatizar respuestas criticas sin control humano.
  - Usar OSINT sin validar fuentes ni marco legal.

### 2.6) Glosario minimo (terminos y definiciones cortas)

- **IoC:** Indicador tecnico de posible compromiso (IP, hash, dominio, etc.).
- **IoA:** Indicador de comportamiento de ataque (acciones/tacticas).
- **SOC:** Centro de operaciones de seguridad.
- **SIEM:** Plataforma de gestion/correlacion de eventos de seguridad.
- **SOAR:** Orquestacion y automatizacion de respuesta.
- **IMS:** Sistema de gestion de incidentes/casos.
- **Playbook:** Flujo guiado de investigacion/respuesta para un tipo de alerta.
- **Runbook:** Procedimiento operativo paso a paso.
- **EPS:** Eventos por segundo en ingesta de logs.
- **Triage:** Clasificacion inicial de alertas para decidir prioridad/escalado.
- **TP/FP:** Verdadero positivo / falso positivo.
- **OSINT:** Inteligencia obtenida de fuentes abiertas y legales.
- **Footprinting:** Recoleccion de huella digital de un objetivo.
- **MITRE ATT&CK:** Marco para mapear tacticas y tecnicas de adversarios.
- **MTTD/MTTR:** Tiempo medio de deteccion / respuesta.

## 3) (Opcional) Evidencias y recursos usados

- [Documentacion de la unidad dos - https://revilofe.github.io/section2/u02/](https://revilofe.github.io/section2/u02/)

## 4) Conclusion (cierre)

En conclusion, esta unidad me ha ayudado a entender mejor como se trabaja un incidente de seguridad de principio a fin, no solo detectando alertas, sino tambien clasificando, priorizando, investigando y documentando cada paso con criterio. Me llevo como idea principal que la eficacia en ciberseguridad no depende solo de tener buenas herramientas, sino de aplicar procesos claros, mantener una buena trazabilidad y aprender de cada caso para mejorar de forma continua.
