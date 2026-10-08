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
