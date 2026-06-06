# Guía completa de clase: Preservación forense

## 1. Datos generales

**Curso:** Informática Forense Aplicada  
**Tema:** Preservación forense  
**Modalidad:** Clase sincrónica, presencial o virtual  
**Duración sugerida:** 2 horas  
**Nivel:** Introductorio/intermedio  
**Público objetivo:** Estudiantes de informática, ciberseguridad, derecho informático, criminología digital o investigación tecnológica.

## 2. Propósito de la clase

Esta clase tiene como finalidad que el estudiante comprenda la importancia de preservar correctamente la evidencia digital para que pueda ser analizada, documentada y eventualmente presentada en un proceso judicial o administrativo sin que su integridad sea cuestionada.

La preservación forense no consiste únicamente en copiar archivos. Es un proceso técnico, metodológico y documental que busca proteger la evidencia desde el momento de su identificación hasta su análisis y presentación.

## 3. Objetivo general

Al finalizar la clase, el estudiante será capaz de explicar y aplicar principios básicos de preservación forense para proteger evidencia digital, garantizar su integridad y documentar adecuadamente el proceso de adquisición.

## 4. Objetivos específicos

Al terminar la sesión, el estudiante podrá:

1. Definir qué es la preservación forense.
2. Explicar por qué la integridad de la evidencia digital es fundamental.
3. Diferenciar entre imágenes lógicas y copias bit a bit.
4. Reconocer el uso de bloqueadores de escritura de hardware y software.
5. Comprender la importancia de la memoria volátil en una investigación.
6. Usar el concepto de hash para verificar integridad.
7. Identificar buenas prácticas para la recolección de evidencia digital.
8. Elaborar un plan básico de adquisición forense.
9. Relacionar la preservación de evidencia con su admisibilidad legal.

## 5. Resultados de aprendizaje esperados

Al finalizar la clase, el estudiante deberá ser capaz de:

- Describir los pasos básicos para preservar una evidencia digital.
- Justificar cuándo conviene usar una copia bit a bit o una imagen lógica.
- Explicar la función de un bloqueador de escritura.
- Interpretar el propósito de un hash MD5 o SHA-256.
- Completar una plantilla básica de cadena de custodia.
- Proponer medidas para reducir riesgos durante una adquisición forense.

## 6. Materiales requeridos

Para el docente:

- Presentación del tema.
- Computadora con acceso a herramientas forenses.
- Ejemplo de memoria USB con datos de prueba.
- Plantilla de cadena de custodia.
- Plantilla de plan de adquisición.
- Proyector o pantalla compartida.

Para los estudiantes:

- Computadora personal, si la clase incluye práctica.
- Acceso a FTK Imager u otra herramienta de adquisición forense.
- Documento de trabajo para completar el plan de adquisición.
- Memoria USB de prueba, no de uso personal ni con información real sensible.

## 7. Distribución sugerida del tiempo

| Bloque | Tema | Duración |
|---|---:|---:|
| 1 | Introducción a la preservación forense | 10 min |
| 2 | Integridad de la evidencia digital | 15 min |
| 3 | Bloqueadores de escritura | 15 min |
| 4 | Copias bit a bit e imágenes lógicas | 15 min |
| 5 | Memoria volátil y captura en vivo | 20 min |
| 6 | Algoritmos hash | 15 min |
| 7 | Marco legal y buenas prácticas | 10 min |
| 8 | Actividad práctica: plan de adquisición | 25 min |
| 9 | Demostración o práctica con FTK Imager | 25 min |
| 10 | Cierre y evaluación rápida | 10 min |

Duración total sugerida: 2 horas y 40 minutos.  
Si la clase debe durar solo 2 horas, se recomienda reducir la práctica con FTK Imager a una demostración guiada.

## 8. Inicio de la clase

### 8.1 Activación de conocimientos previos

Inicie la clase con preguntas breves:

- ¿Qué creen que puede pasar si se manipula mal una computadora usada como evidencia?
- ¿Una captura de pantalla puede considerarse prueba?
- ¿Qué diferencia hay entre copiar archivos y preservar evidencia?
- ¿Por qué podría rechazarse una evidencia digital en un juicio?

### 8.2 Idea introductoria

Explique que la evidencia digital es frágil. Puede modificarse con acciones simples como encender un equipo, abrir un archivo, conectar una memoria USB o copiar datos sin protección. Por eso la informática forense necesita procedimientos claros y documentados.

Mensaje clave para el docente:

> Una evidencia digital puede contener información importante, pero si no fue preservada correctamente, puede perder valor técnico y legal.

## 9. Desarrollo teórico

### 9.1 Introducción a la preservación forense

La preservación forense es el conjunto de procedimientos utilizados para garantizar que una evidencia digital conserve su estado original durante una investigación.

Este proceso permite:

- Evitar alteraciones accidentales o intencionales.
- Proteger la integridad de la información.
- Mantener trazabilidad sobre quién tuvo acceso a la evidencia.
- Asegurar que la evidencia pueda ser explicada y defendida.
- Facilitar su admisibilidad en un proceso judicial.

Aspectos esenciales:

- Usar herramientas adecuadas y certificadas cuando sea posible.
- Documentar cada acción realizada.
- Trabajar sobre copias forenses, no sobre el dispositivo original.
- Calcular valores hash antes y después de la adquisición.
- Mantener cadena de custodia.

Ejemplo para explicar:

Un empleado es sospechoso de filtrar información confidencial mediante una memoria USB. Si el investigador conecta la USB directamente a su computadora y abre archivos, podría modificar metadatos, fechas de acceso o archivos ocultos. Esto puede generar dudas sobre la autenticidad de la evidencia.

### 9.2 Importancia de la integridad de la evidencia

La integridad significa que la evidencia no ha sido alterada desde su recolección hasta su análisis y presentación.

Para garantizarla, se recomienda:

- Establecer protocolos claros.
- Usar bloqueadores de escritura.
- Calcular hashes.
- Registrar fecha, hora y responsable de cada acción.
- Conservar el dispositivo original en condiciones seguras.

Características esperadas de una evidencia digital:

| Característica | Descripción |
|---|---|
| Admisible | Cumple con requisitos legales y procedimentales. |
| Auténtica | Tiene relación directa con el hecho investigado. |
| Completa | Permite comprender el caso de manera integral. |
| Confiable | Fue recolectada y procesada con métodos verificables. |
| Creíble | Puede ser explicada de forma clara ante terceros. |

Pregunta de discusión:

¿Por qué una evidencia técnicamente correcta podría ser rechazada?

Respuesta esperada:

Porque no se documentó correctamente, se rompió la cadena de custodia, no se usaron herramientas adecuadas o no se puede demostrar que no fue alterada.

### 9.3 Sistemas de protección contra escritura

Los sistemas de protección contra escritura impiden que se modifique el contenido de un dispositivo durante su adquisición o análisis.

#### Bloqueadores de hardware

Son dispositivos físicos que se colocan entre la computadora del analista y el medio de almacenamiento.

Ejemplos:

- Forensic UltraDock.
- Tableau T35u.

Ventajas:

- Mayor confiabilidad.
- Reducción del riesgo de escritura accidental.
- Uso frecuente en laboratorios forenses.

#### Bloqueadores de software

Son herramientas o configuraciones que permiten acceder al dispositivo en modo solo lectura.

Ejemplo:

- FTK Imager.

Ventajas:

- Son más accesibles para prácticas académicas.
- Pueden ser suficientes en entornos controlados.
- Permiten crear y verificar imágenes forenses.

Consideraciones antes de usarlos:

- Verificar compatibilidad con el dispositivo.
- Realizar pruebas previas.
- Configurar correctamente la herramienta.
- Documentar errores, advertencias o comportamientos inesperados.

### 9.4 Copias bit a bit e imágenes lógicas

Es importante distinguir entre copiar archivos visibles y adquirir una imagen forense completa.

| Aspecto | Imagen lógica | Copia bit a bit |
|---|---|---|
| Alcance | Archivos visibles o seleccionados. | Todo el contenido del dispositivo. |
| Espacio no asignado | Normalmente no lo incluye. | Sí lo incluye. |
| Archivos eliminados | Recuperación limitada. | Puede permitir recuperación. |
| Velocidad | Más rápida. | Más lenta. |
| Uso recomendado | Búsqueda rápida y específica. | Investigación exhaustiva. |

Explicación sencilla:

- Una imagen lógica es como copiar las carpetas visibles.
- Una copia bit a bit es como clonar todo el dispositivo, incluyendo áreas no visibles, archivos eliminados y estructuras internas.

Pregunta para estudiantes:

Si se sospecha que un usuario eliminó archivos antes de entregar su computadora, ¿qué tipo de adquisición conviene usar?

Respuesta esperada:

Una copia bit a bit.

### 9.5 Memoria volátil

La memoria RAM almacena información temporal que desaparece cuando el equipo se apaga o reinicia.

Puede contener:

- Procesos en ejecución.
- Conexiones de red activas.
- Claves de cifrado.
- Fragmentos de archivos abiertos.
- Credenciales temporales.
- Evidencia de malware en ejecución.

Idea clave:

Si el equipo está encendido, se debe evaluar si conviene capturar la memoria RAM antes de apagarlo.

Ejemplo:

Si un equipo comprometido tiene malware ejecutándose, apagarlo puede eliminar información clave sobre el proceso malicioso, sus conexiones o su comportamiento.

### 9.6 Captura en sistemas operativos en vivo

La captura en vivo permite adquirir evidencia de un sistema encendido. Puede ser necesaria cuando hay información volátil o cuando apagar el equipo puede causar pérdida de evidencia.

Buenas prácticas:

- Documentar fecha y hora.
- Registrar usuario responsable.
- Registrar herramientas utilizadas.
- Anotar comandos ejecutados.
- Registrar cualquier cambio observado.
- Justificar por qué se realizó captura en vivo.

Riesgo principal:

Cualquier acción realizada sobre un sistema encendido puede modificar información. Por eso debe justificarse y documentarse.

### 9.7 Algoritmos hash

Un hash es una huella digital generada a partir de datos. Si los datos cambian, el hash también cambia.

Algoritmos comunes:

- MD5.
- SHA-1.
- SHA-256.

Uso en informática forense:

- Verificar que una copia sea idéntica al original.
- Validar imágenes forenses.
- Detectar alteraciones.
- Comparar evidencia durante el análisis.

Ejemplo:

Archivo original:

```text
contrato.pdf
SHA-256: A1B2C3D4...
```

Si se modifica una sola letra dentro del archivo, el hash resultante será diferente.

Recomendación:

Aunque MD5 todavía aparece en muchos reportes forenses por compatibilidad, SHA-256 es una opción más robusta para verificar integridad.

### 9.8 Herramientas de preservación

Herramientas de hardware:

- Tableau T35u.
- Forensic UltraDock.
- Otros bloqueadores de escritura certificados.

Herramientas de software:

- FTK Imager.
- Herramientas de cálculo hash.
- Sistemas operativos forenses ejecutados desde medios externos.

Buenas prácticas:

- Mantener herramientas actualizadas.
- Usar versiones confiables.
- Probar los equipos antes de una adquisición real.
- Documentar configuración y versión utilizada.

### 9.9 Marco legal: Costa Rica

El material menciona la Ley 9048, Delitos Informáticos y Conexos, relacionada con la penalización de delitos como acceso no autorizado, fraude informático, sabotaje, alteración de datos y otros comportamientos vinculados con sistemas de información.

Punto importante para la clase:

El análisis técnico debe ajustarse a requisitos legales. No basta con encontrar evidencia; también debe poder demostrarse cómo se obtuvo, cómo se protegió y cómo se mantuvo íntegra.

## 10. Actividad práctica 1: Plan de adquisición

### Escenario

Un empleado de una empresa es sospechoso de filtrar información confidencial a través de su correo electrónico personal y un dispositivo USB.

### Instrucciones

Los estudiantes deben elaborar un plan de adquisición que incluya:

1. Dispositivos identificados.
2. Herramientas para su análisis.
3. Protocolo de adquisición.
4. Cadena de custodia.
5. Riesgos asociados.
6. Medidas de mitigación.

### Guía de respuesta esperada

#### Dispositivos identificados

- Computadora del empleado.
- Memoria USB.
- Cuenta de correo electrónico, si existe autorización legal.
- Registros del sistema.
- Logs de proxy, firewall o servidor de correo.
- Carpetas compartidas o unidades de red.

#### Herramientas

- FTK Imager.
- Bloqueador de escritura.
- Herramienta de cálculo hash.
- Plantilla de cadena de custodia.
- Cámara o teléfono institucional para documentar estado físico.
- Software de análisis forense.

#### Protocolo sugerido

1. Asegurar el área.
2. Fotografiar dispositivos y conexiones.
3. Registrar fecha, hora y responsables.
4. Identificar si el equipo está encendido o apagado.
5. Evaluar captura de memoria RAM.
6. Usar bloqueador de escritura para medios extraíbles.
7. Crear imagen forense.
8. Calcular hash del original y de la copia.
9. Comparar hashes.
10. Etiquetar evidencia.
11. Almacenar en lugar seguro.
12. Documentar cada paso.

#### Riesgos y mitigación

| Riesgo | Mitigación |
|---|---|
| Alteración accidental | Usar bloqueador de escritura. |
| Pérdida de memoria volátil | Capturar RAM antes de apagar, si aplica. |
| Falta de autorización | Verificar permisos legales o institucionales. |
| Evidencia incompleta | Preferir adquisición bit a bit cuando sea necesario. |
| Ruptura de cadena de custodia | Registrar cada transferencia. |
| Confusión de evidencias | Etiquetar claramente cada dispositivo. |

### Producto esperado

Cada grupo debe entregar un plan breve de adquisición de una a dos páginas y explicar sus decisiones principales.

## 11. Actividad práctica 2: Imagen forense con FTK Imager

Esta actividad puede realizarse como práctica individual, práctica grupal o demostración del docente.

### Materiales

- Computadora con FTK Imager instalado.
- Memoria USB con datos de prueba.
- Carpeta de destino para guardar la imagen.
- Formato de registro de evidencia.

### Procedimiento

1. Abrir FTK Imager.
2. Seleccionar `File > Create Disk Image`.
3. Elegir `Physical Drive`.
4. Seleccionar la memoria USB conectada.
5. Completar los datos del caso:
   - Número de caso.
   - Nombre del investigador.
   - Descripción de la evidencia.
   - Fecha y hora.
   - Observaciones.
6. Seleccionar formato E01.
7. Habilitar verificación hash.
8. Especificar ubicación de almacenamiento.
9. Iniciar el proceso.
10. Esperar la finalización.
11. Verificar que el hash generado coincida.
12. Guardar el reporte de adquisición.

### Preguntas posteriores

- ¿Por qué no se debe analizar directamente la memoria USB original?
- ¿Qué representa el hash generado?
- ¿Qué pasaría si el hash de la imagen no coincide con el original?
- ¿Qué datos deben documentarse en el reporte?

## 12. Evaluación de aprendizaje

### Opción A: Preguntas rápidas

1. ¿Qué es la preservación forense?
2. ¿Para qué sirve un bloqueador de escritura?
3. ¿Cuál es la diferencia entre imagen lógica y copia bit a bit?
4. ¿Por qué es importante la memoria volátil?
5. ¿Qué función cumple un hash?
6. ¿Qué información debe contener una cadena de custodia?

### Opción B: Caso breve

Caso:

> Una computadora fue incautada por sospecha de fraude. El investigador la encendió, revisó archivos, copió algunos documentos a su memoria USB personal y luego entregó la computadora como evidencia.

Preguntas:

- ¿Qué errores cometió el investigador?
- ¿Cómo debió actuar?
- ¿La evidencia podría ser cuestionada?
- ¿Qué procedimiento habría reducido el riesgo?

Respuesta esperada:

La evidencia podría ser cuestionada porque hubo manipulación directa, no se usó bloqueador de escritura, no se generaron hashes, no se documentó correctamente el procedimiento y se utilizó una memoria personal.

## 13. Cierre de la clase

Ideas principales para reforzar:

- La preservación forense protege la evidencia digital.
- La integridad es esencial para la admisibilidad.
- La documentación es tan importante como la técnica.
- Los hashes permiten verificar que la evidencia no fue alterada.
- La cadena de custodia permite demostrar trazabilidad.
- Una adquisición incorrecta puede comprometer toda la investigación.

Frase de cierre:

> En informática forense, no basta con encontrar la evidencia; hay que demostrar que fue obtenida, preservada y analizada correctamente.

## 14. Plantilla básica de cadena de custodia

| Campo | Información |
|---|---|
| Número de caso | |
| Descripción de evidencia | |
| Tipo de dispositivo | |
| Marca/modelo | |
| Número de serie | |
| Fecha y hora de recolección | |
| Lugar de recolección | |
| Nombre del recolector | |
| Hash MD5 | |
| Hash SHA-256 | |
| Estado físico del dispositivo | |
| Persona que entrega | |
| Persona que recibe | |
| Firma | |
| Observaciones | |

## 15. Rúbrica sugerida para evaluar el plan de adquisición

| Criterio | Excelente | Aceptable | Requiere mejora |
|---|---|---|---|
| Identificación de evidencia | Identifica todos los dispositivos relevantes. | Identifica los principales. | Omite evidencia importante. |
| Selección de herramientas | Herramientas adecuadas y justificadas. | Herramientas adecuadas sin mucha justificación. | Herramientas inadecuadas o ausentes. |
| Protocolo de adquisición | Ordenado, completo y seguro. | Tiene pasos básicos. | Presenta vacíos críticos. |
| Cadena de custodia | Completa y trazable. | Parcialmente documentada. | Insuficiente o confusa. |
| Gestión de riesgos | Riesgos claros con mitigaciones viables. | Menciona algunos riesgos. | No identifica riesgos relevantes. |

## 16. Referencias base

- Donohue, B. (2014). ¿Qué es un HASH y cómo funciona? Kaspersky.
- Gitlan, D. (2024). Qué es el algoritmo SHA-256 y cómo funciona. SSL Dragon.
- Pcweb.info. (2023). Memoria volátil y no volátil: qué es, definición.
- Poder Judicial de Costa Rica. (s. f.). La evidencia digital en el combate contra la ciberdelincuencia.
- Ley 9048, Delitos Informáticos y Conexos, Costa Rica.
