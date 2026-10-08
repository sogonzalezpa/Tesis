# Validación

## Comparadores

- Método analítico convencional.
- LLM sin herramientas.
- LLM con recuperación de evidencia.
- Flujo fijo con herramientas.
- Sistema agéntico.
- Multiagente: incluir solo con justificación.

## Control experimental

- Mismo modelo, corpus y tareas cuando sea posible.
- Registrar presupuesto de tokens y herramientas.
- Comparar también coste y tiempo.
- Repetir ejecuciones.
- Separar diseño, ajuste y prueba.
- Ablaciones: retirar recuperación, verificación o coordinación.
- Casos con evidencia contradictoria y datos faltantes.
- Congelar corpus, versiones y configuraciones.
- Evaluar filtraciones de información futura.

## Métricas

- Exactitud de extracción y cálculo.
- Cumplimiento de restricciones.
- Fidelidad de citas y cobertura de evidencia.
- Calidad de alternativas y sensibilidad.
- Equidad: criterio explícito del caso.
- Estabilidad, tiempo y coste.
- Abstención ante evidencia insuficiente.
- Juicio experto: rúbrica y evaluación ciega cuando sea factible.
- No usar solo otro LLM como juez.
- No atribuir impacto causal a recomendaciones simuladas.

## 2026-10-08 — Validar la metodología

- Unidad principal: proyecto/equipo que desarrolla una solución.
- Ejecuciones del agente: observaciones técnicas anidadas; no proyectos independientes.
- Comparar procedimiento base y procedimiento propuesto.
- Base: metodología analítica existente más guía pública pertinente.
- Evitar comparador débil sin prácticas mínimas.
- Mantener herramientas, modelos, presupuesto y tareas comparables.
- Diseño por equipos o cruzado; controlar aprendizaje y experiencia.
- Predefinir hipótesis, métrica primaria y mejora relevante.
- Tamaño muestral: estimar con piloto; no inventar número obligatorio.
- Evaluación ciega de productos cuando sea posible.
- Registrar fidelidad de aplicación y esfuerzo de documentación.
- Informar intervalos de incertidumbre y fallos, no solo promedios.
- Separar efecto de procedimiento, tecnología y experiencia del equipo.

## Validación en tres niveles

- Contenido: expertos revisan coherencia, cobertura y aplicabilidad.
- Ejecución: equipos distintos aplican instrucciones y producen artefactos.
- Resultado: comparaciones controladas de calidad, tiempo, coste y trazabilidad.
- Validación experta sola: insuficiente para eficacia.
- Prototipo exitoso solo: insuficiente para metodología transferible.
- Varias ejecuciones del mismo prototipo: insuficientes para generalización.

## Casos candidatos

- Caso A: convertir documentos públicos en indicadores trazables.
- Caso B: combinar datos e indicadores para predicción o priorización.
- Elegir según disponibilidad, referencia verificable y viabilidad.
- Transferencia: otra tarea, conjunto de datos o equipo no usado en diseño.
- Casos retrospectivos y datos abiertos permiten evaluación técnica.
- Sin participantes/uso real: no concluir usabilidad institucional ni impacto público.
- Simulación: probar restricciones y estabilidad; no impacto causal real.

## Criterios para revisar o abandonar

- Si proceso existente cubre todas las reglas: justificar extensión mínima o reformular.
- Si solo mejora el modelo/arquitectura: aporte metodológico no demostrado.
- Si documentación cuesta más sin beneficio verificable: revisar utilidad.
- Si agentes no mejoran frente a flujo fijo: conservar resultado negativo.
- Si solo funciona en un caso: limitar alcance y generalización.
