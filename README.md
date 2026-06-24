# Implementación de un sistema de pruebas de progresión de estado

En un sistema de banca digital, es crucial garantizar que las solicitudes de los clientes progresen correctamente a través de las diferentes etapas de procesamiento. Este reto se centra en la implementación de un sistema de pruebas que verifica la progresión del estado de una solicitud a través de un pipeline de procesamiento. Los actores involucrados son el cliente, el sistema de gestión de solicitudes y el motor de procesamiento. Las propiedades operativas incluyen la consistencia del estado entre el sistema de gestión y el motor de procesamiento, con un umbral de latencia de 2 segundos para la actualización del estado. La razón de negocio es asegurar que las solicitudes se procesen de manera eficiente y que los clientes reciban actualizaciones precisas y oportunas.

## Informacion General

| Campo | Valor |
|-------|-------|
| **Tema** | Status Progression Test |
| **Nivel** | junior-l2 |
| **Tipo** | practical |
| **Tiempo estimado** | 8 horas |

## Fases del Reto

### Fase 0: Configuración del Proyecto

**Objetivo:** Obtener el proyecto base funcional enviando el Código Base a un asistente de IA, que lo analizará, corregirá errores y generará un ZIP listo para usar.

**Tiempo estimado:** 15-30 minutos

**Instrucciones:**

- Asegúrate de tener instalado para ejecutar el proyecto: Un IDE o editor de código.
- Copia todo el contenido del campo **Código Base** de este reto — incluyendo el texto de instrucciones que aparece al inicio.
- Abre un asistente de IA (Claude en claude.ai, ChatGPT o Gemini — se recomienda Claude), pega el contenido copiado en el chat y envíalo.
- El asistente analizará los archivos, corregirá errores y generará un archivo ZIP descargable. Descárgalo y extráelo en la carpeta donde quieras trabajar.
- Verifica que el proyecto arranca sin errores.

**Entregable:** El proyecto compila/arranca sin errores.

<details>
<summary>Pistas de conocimiento</summary>

- Copia el Código Base completo incluyendo el texto de instrucciones al inicio — esas instrucciones le indican al asistente exactamente qué hacer con los archivos.
- Si el asistente no genera el ZIP automáticamente al terminar el análisis, escríbele: "genera el ZIP ahora".
- Si el proyecto tiene errores al arrancar, comparte el mensaje de error con el mismo asistente para que lo corrija.

</details>

### Fase 1: Configuración del entorno de pruebas

**Objetivo:** Establecer un entorno de pruebas que permita simular la progresión del estado de una solicitud.

**Tiempo estimado:** 2 horas

**Instrucciones:**

- Identificar los componentes y actores involucrados en la progresión del estado de una solicitud.
- Definir los criterios de aceptación para la configuración del entorno de pruebas.

**Entregable:** Entorno de pruebas configurado con los componentes y actores necesarios.

<details>
<summary>Pistas de conocimiento</summary>

- Considera la interacción entre el cliente, el sistema de gestión de solicitudes y el motor de procesamiento.
- Piensa en cómo simular la latencia y los posibles fallos en la actualización del estado.

</details>

### Fase 2: Implementación de pruebas unitarias

**Objetivo:** Desarrollar pruebas unitarias que verifiquen la correcta progresión del estado de una solicitud.

**Tiempo estimado:** 3 horas

**Instrucciones:**

- Crear pruebas unitarias para cada etapa de la progresión del estado.
- Asegurar que las pruebas cubran los casos de éxito y los casos de error.

**Entregable:** Conjunto de pruebas unitarias implementadas y ejecutadas con éxito.

<details>
<summary>Pistas de conocimiento</summary>

- Considera los diferentes estados por los que puede pasar una solicitud y las transiciones entre ellos.
- Piensa en cómo simular errores y fallos en la progresión del estado.

</details>

### Fase 3: Integración de pruebas de progresión de estado

**Objetivo:** Integrar las pruebas de progresión de estado en el pipeline de CI/CD.

**Tiempo estimado:** 3 horas

**Instrucciones:**

- Configurar el pipeline de CI/CD para ejecutar las pruebas de progresión de estado.
- Asegurar que las pruebas se ejecuten automáticamente en cada commit.

**Entregable:** Pipeline de CI/CD configurado para ejecutar automáticamente las pruebas de progresión de estado.

<details>
<summary>Pistas de conocimiento</summary>

- Considera la configuración del pipeline para que las pruebas se ejecuten de manera eficiente y no bloqueen el proceso de integración continua.
- Piensa en cómo notificar los resultados de las pruebas a los desarrolladores.

</details>

## Dimensiones Evaluadas

- **queEs**: ¿Qué es la progresión de estado en el contexto de un sistema de banca digital?
- **paraQueSirve**: ¿Para qué sirven las pruebas de progresión de estado en un pipeline de procesamiento?
- **comoSeUsa**: ¿Cómo se usan las pruebas unitarias para verificar la correcta progresión del estado de una solicitud?
- **erroresComunes**: ¿Cuáles son los errores comunes que pueden ocurrir durante la progresión del estado de una solicitud?
- **queDecisionesImplica**: ¿Qué decisiones implica la integración de pruebas de progresión de estado en un pipeline de CI/CD?

## Criterios de Evaluacion

- Configuración correcta del entorno de pruebas.
- Implementación de pruebas unitarias que cubran casos de éxito y error.
- Integración exitosa de las pruebas en el pipeline de CI/CD.

---

*Reto generado automaticamente por Challenge Generator - Pragma*
