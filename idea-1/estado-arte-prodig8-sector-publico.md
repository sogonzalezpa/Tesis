# Estado preliminar del arte y viabilidad de una adaptación de PRODIG8 para el sector público

**Repositorio:** `sogonzalezpa/Tesis`  
**Carpeta:** `idea-1`  
**Fecha de corte:** 1 de octubre de 2026  
**Propósito:** establecer si es científicamente, metodológicamente y administrativamente viable convertir PRODIG8 en una metodología de *government analytics*, dentro de las restricciones de la Convocatoria 35 y el proyecto BPIN 2024000100132. La propuesta presentada para la admisión al Doctorado en Ingeniería—Sistemas e Informática de la Universidad Nacional de Colombia se considera un antecedente orientador, no una fuente vinculante de restricciones para la tesis.

## 1. Pregunta de decisión

La pregunta que orienta este estado preliminar del arte es:

> ¿Existe un vacío metodológico suficientemente claro en la ejecución de proyectos de analítica para entidades públicas que justifique adaptar y validar PRODIG8, manteniendo la articulación con las demandas territoriales y los objetivos de la Convocatoria 35?

La decisión no consiste todavía en cambiar la tesis. Consiste en determinar si la idea tiene una base científica defendible y qué condiciones debe cumplir frente a la convocatoria de la beca. La adscripción doctoral en Ingeniería—Sistemas e Informática, Facultad de Minas, delimita el campo científico hacia analytics; el estado del arte permite denominar el ámbito de aplicación como *government analytics*.

## 2. Alcance y estrategia de búsqueda

Se realizó una búsqueda exploratoria en:

- Google Scholar mediante búsquedas de título, resumen y términos relacionados;
- OpenAlex, para identificar trabajos académicos, DOI, años de publicación y redes temáticas;
- sitios oficiales de OECD, World Bank, MinCiencias y la Universidad Autónoma de Manizales;
- bases y resultados indexados visibles en Scopus, Web of Science, IEEE, ScienceDirect, Springer, SAGE, MDPI, PeerJ y revistas de administración pública;
- el artículo **“Strategies for Executing Analytics Projects: Toward a Unified Framework of Methodologies”**, disponible en `idea-1/prodig8.docx`.

Las cadenas exploratorias incluyeron:

- “public sector analytics”;
- “government analytics”;
- “data-driven decision-making public sector”;
- “public sector analytics methodology”;
- “CRISP-DM government”;
- “AI governance public sector”;
- “fair allocation public resources”;
- “public policy big data analytics”;
- “analytics project lifecycle public administration”.

La búsqueda es preliminar, no una revisión sistemática cerrada. Por ello, las conclusiones sobre novedad deben confirmarse mediante un protocolo reproducible con PRISMA 2020, criterios de inclusión y exclusión, búsqueda por bases y revisión de referencias y citas.

## 3. Definición de analítica en el sector público

La definición operativa más útil para esta investigación es:

> La analítica en el sector público es el uso sistemático de datos administrativos, territoriales, sociales, económicos y ciudadanos, junto con métodos estadísticos, de inteligencia artificial, investigación de operaciones y visualización, para comprender problemas públicos, anticipar escenarios, evaluar alternativas y apoyar decisiones institucionales orientadas al valor público, la equidad, la legalidad y la rendición de cuentas.

Esta definición tiene cinco componentes:

1. **Datos públicos y de interés público.** Incluye registros administrativos, censos, datos abiertos, información geoespacial, encuestas, datos de programas sociales y, cuando sea legal y técnicamente posible, datos aportados por organizaciones aliadas.
2. **Ciclo analítico completo.** Comprende analítica descriptiva, diagnóstica, predictiva y prescriptiva. No se limita a tableros o modelos predictivos.
3. **Decisión institucional.** El resultado debe apoyar una política, programa, servicio, asignación, inspección, prevención o evaluación; no basta con producir una métrica.
4. **Valor público.** La eficiencia es insuficiente. También deben considerarse equidad, inclusión, transparencia, derechos, confianza, sostenibilidad y resultados para la ciudadanía.
5. **Responsabilidad pública.** Las decisiones requieren trazabilidad, control humano, explicación, protección de datos, gestión de riesgos, participación de actores y mecanismos de reclamación o revisión.

El Banco Mundial define government analytics como el uso de datos para diagnosticar y mejorar el funcionamiento del gobierno o de la administración pública. La OECD, por su parte, presenta los datos como un activo estratégico para diseñar políticas, prestar servicios y evaluar resultados, pero advierte que el valor depende de gobernanza, interoperabilidad, capacidades y confianza.

Por tanto, la analítica pública no es simplemente “business analytics aplicada al gobierno”. Cambia el objetivo de optimización: en el sector privado suele priorizar rentabilidad, mientras que en el sector público debe equilibrar eficiencia, equidad, derechos, legalidad, cobertura y legitimidad.

## 4. ¿Existen metodologías para decisiones basadas en datos en el sector público?

### 4.1 Metodologías generales de analítica

La literatura técnica cuenta con metodologías consolidadas:

- **KDD:** descubrimiento de conocimiento a partir de datos.
- **CRISP-DM:** comprensión del negocio, comprensión de datos, preparación, modelado, evaluación y despliegue.
- **SEMMA:** muestra, explora, modifica, modela y evalúa.
- **ASUM-DM:** amplía CRISP-DM con gestión de proyectos, comunicación y coordinación.
- **TDSP:** integra ciencia de datos, ingeniería de software, control de versiones, automatización y despliegue.
- **OSEMN:** obtener, limpiar, explorar, modelar e interpretar.
- **INFORMS Analytics Process:** formulación del problema de negocio, problema analítico, datos, metodología, construcción, despliegue y ciclo de vida.
- **CRISP-ML(Q):** añade aseguramiento de calidad, reproducibilidad y mantenimiento de modelos.
- **DMME, DataPro y MAISTRO:** incorporan comprensión técnica, implementación, operación, mantenimiento, ética y mejora continua.

Estas metodologías aportan una base fuerte para PRODIG8. Sin embargo, la mayoría surgió en contextos empresariales, industriales, tecnológicos o de ciencia de datos. Incluso cuando se aplican en gobiernos, suelen adaptar una metodología existente a un caso particular y no siempre producen una metodología pública generalizable.

### 4.2 Evidencia de adaptación al sector público

La literatura sí demuestra que la analítica se usa en:

- salud pública y vigilancia epidemiológica;
- educación y riesgo de deserción;
- tributación y detección de fraude;
- seguridad y gestión de riesgos;
- movilidad y transporte;
- focalización de programas sociales;
- planeación urbana;
- gestión de recursos y prestación de servicios;
- evaluación de políticas públicas.

También existen marcos de gobierno digital, datos públicos, inteligencia artificial responsable, evaluación de impacto algorítmico y toma de decisiones basada en evidencia. No obstante, estos marcos cumplen funciones diferentes:

- algunos son principios éticos;
- otros son guías de datos;
- otros son ciclos de política pública;
- otros son metodologías técnicas de machine learning;
- otros son modelos de madurez institucional.

La evidencia preliminar muestra una fragmentación: pocos marcos integran en un mismo ciclo la formulación del problema público, la gobernanza de datos, el diseño analítico, la equidad, la participación, la implementación institucional, la evaluación de impacto y la mejora continua.

### 4.3 Principales limitaciones identificadas

La revisión preliminar permite agrupar las limitaciones en seis categorías:

| Categoría | Problema recurrente |
|---|---|
| Datos | fragmentación, baja calidad, falta de interoperabilidad, sesgos de cobertura y datos no actualizados |
| Organización | silos institucionales, falta de roles, baja capacidad analítica y dependencia de proveedores |
| Método | metodologías centradas en el modelo, con poca conexión entre problema público, decisión y resultado |
| Gobernanza | responsabilidades difusas, baja trazabilidad, ausencia de auditoría y débil control humano |
| Derechos | privacidad, sesgo, discriminación, explicabilidad, debido proceso y posibilidad de reclamación |
| Sostenibilidad | modelos que no se mantienen, falta de monitoreo, deriva de datos, presupuesto y apropiación institucional |

Estas limitaciones son relevantes para la asignación de subsidios o recursos sociales, porque un modelo técnicamente preciso puede producir decisiones injustas si los datos históricos contienen filtración, subcobertura o discriminación territorial.

## 5. Qué aporta PRODIG8

El artículo de PRODIG8 propone una arquitectura de ocho dimensiones organizada en tres funciones:

### Ejecución

1. definición del alcance del proyecto;
2. comprensión de datos;
3. preparación de datos;
4. diseño del proyecto;
5. evaluación del modelo;
6. operación y mantenimiento.

### Control transversal

7. gobernanza y ética.

### Adaptación

8. mejora continua.

El aporte de PRODIG8 no consiste únicamente en ordenar fases técnicas. Su principal valor es integrar ejecución, control y adaptación. Esa estructura es compatible con los problemas del sector público, especialmente porque incluye gobernanza, ética, operación y aprendizaje.

El artículo también identifica una fragmentación de metodologías y muestra que los marcos existentes difieren en el tratamiento de gestión de proyectos, implementación, mantenimiento, ética, gobernanza y retroalimentación. Esa conclusión ofrece una base sólida para estudiar una extensión pública.

## 6. Aportes y modificaciones necesarias para una versión pública

La adaptación no debería llamarse simplemente “PRODIG8 aplicado al sector público”. Para constituir una contribución doctoral debe explicar qué cambia en cada dimensión y por qué esos cambios son necesarios.

### 6.1 Definición del problema y alcance público

Cambiar la comprensión de negocio por **formulación del problema público y teoría de cambio**.

Debe incluir:

- problema social verificable;
- población afectada;
- autoridad competente;
- instrumento de política pública;
- decisión que el modelo apoyará;
- restricciones legales, presupuestales y territoriales;
- resultados esperados para la ciudadanía;
- riesgos de no intervención;
- actores que pueden beneficiarse o verse perjudicados.

### 6.2 Gobernanza pública de datos

Ampliar la comprensión de datos con:

- autoridad y finalidad del tratamiento;
- base legal;
- calidad, procedencia y trazabilidad;
- interoperabilidad;
- protección de datos personales;
- retención, acceso y seguridad;
- acuerdos de intercambio;
- documentación de datos faltantes;
- sesgos de representación;
- mecanismos de actualización.

### 6.3 Equidad y derechos como requisitos de diseño

La equidad no debe aparecer solo en la evaluación final. Debe incorporarse desde la definición del problema y medirse durante todo el ciclo.

Posibles criterios:

- igualdad de oportunidades;
- cobertura efectiva;
- filtración y subcobertura;
- paridad entre grupos;
- impacto territorial;
- índice de Gini o Atkinson;
- análisis de sensibilidad;
- distribución de errores;
- trato diferencial justificado;
- posibilidad de revisión humana.

### 6.4 Participación y conocimiento institucional

Agregar una dimensión o subproceso de **co-diseño público**:

- funcionarios responsables;
- población afectada;
- organizaciones sociales;
- expertos temáticos;
- autoridades de protección de datos;
- órganos de control;
- equipos jurídicos y de contratación.

La metodología debe documentar cómo las necesidades y restricciones de estos actores modifican los requisitos analíticos.

### 6.5 Explicabilidad, transparencia y rendición de cuentas

PRODIG8 debe incorporar productos verificables:

- ficha del sistema;
- ficha de datos;
- ficha del modelo;
- registro de decisiones;
- explicación individual y global;
- matriz de riesgos;
- protocolo de incidentes;
- responsable institucional;
- procedimiento de reclamación;
- informe público de limitaciones.

### 6.6 Implementación y sostenibilidad institucional

La operación y mantenimiento deben incluir:

- capacidad tecnológica y humana de la entidad;
- presupuesto de continuidad;
- interoperabilidad con sistemas existentes;
- capacitación;
- gestión del cambio;
- monitoreo de deriva;
- reentrenamiento;
- evaluación de impacto;
- retiro del modelo cuando deje de ser confiable.

### 6.7 Evidencia de impacto público

La metodología debe distinguir entre:

- calidad estadística del modelo;
- calidad de la recomendación;
- cambio en la decisión institucional;
- resultado del programa;
- efecto sobre la población.

Una tesis fuerte no debería concluir que el modelo es exitoso solo porque tiene buen AUC, precisión o error bajo. Debe demostrar si mejora la asignación, reduce desigualdades o disminuye filtración y subcobertura sin vulnerar derechos.

## 7. Viabilidad frente a la Convocatoria 35 y al BPIN 2024000100132

La convocatoria exige que la propuesta doctoral responda a retos de ciencia, tecnología e innovación y a demandas territoriales de Caldas, Risaralda, Quindío o Antioquia. También exige una propuesta de investigación articulada con al menos una demanda territorial.

La adaptación pública de PRODIG8 puede alinearse con la convocatoria si se formula como una investigación aplicada de generación de nuevo conocimiento para fortalecer la toma de decisiones basada en evidencia en Antioquia.

La alineación es especialmente defendible cuando el caso de validación aborda:

- asignación de subsidios o recursos sociales;
- población vulnerable;
- gobernanza territorial;
- transformación digital;
- inclusión y equidad;
- fortalecimiento de capacidades institucionales.

La propuesta debe mantener un problema público concreto. Una metodología abstracta para “cualquier entidad pública” sería débil frente a la convocatoria porque podría parecer un producto general de consultoría. La metodología debe ser construida y validada a partir de un caso territorial real, con posibilidad de transferencia a otros municipios o programas.

## 8. Delimitación recomendada de la tesis

### Título de trabajo

**PRODIG8-Público: metodología de desarrollo, gobernanza y evaluación de proyectos de analítica prescriptiva para la asignación equitativa de recursos sociales en entidades territoriales.**

### Objetivo general propuesto

> Diseñar y validar una adaptación de PRODIG8 para el desarrollo y operación responsable de proyectos de analítica prescriptiva en entidades públicas, incorporando gobernanza de datos, equidad, explicabilidad, participación y evaluación de impacto, mediante un caso de asignación de recursos sociales en Medellín y Antioquia.

### Objetivos específicos propuestos

1. Caracterizar las metodologías de analítica y los marcos de toma de decisiones basadas en datos utilizados en el sector público.
2. Identificar las brechas de CRISP-DM, TDSP, ASUM-DM, INFORMS, CRISP-ML(Q), DataPro, MAISTRO y PRODIG8 frente a las necesidades de las entidades públicas.
3. Diseñar la extensión PRODIG8-Público, con fases, roles, productos, criterios de gobernanza, equidad y evaluación.
4. Aplicar la metodología a un caso de asignación de subsidios, ayudas o recursos sociales para población vulnerable.
5. Validar la metodología mediante evaluación técnica, institucional, ética y de impacto público.

## 9. Regla de alcance doctoral: artefacto, validación y resultados lejanos

Una tesis doctoral no debe prometer simultáneamente desarrollar una metodología, implementarla en una entidad pública y medir efectos sociales o presupuestales definitivos. En *government analytics*, esos efectos pueden depender de ciclos presupuestales, cambios de gobierno, adopción institucional, decisiones jurídicas y comportamiento ciudadano que exceden el horizonte de la tesis.

Por ello, la formulación debe separar tres niveles:

| Nivel | Qué debe hacer la tesis | Qué no debe prometer |
|---|---|---|
| Diseño | construir PRODIG8-Público como artefacto metodológico, con fases, roles, productos, controles y criterios de decisión | afirmar que la metodología ya mejoró una política pública a gran escala |
| Validación | demostrar pertinencia, coherencia, usabilidad, trazabilidad, factibilidad y desempeño en un caso o piloto controlado | atribuir cambios sociales de largo plazo exclusivamente al artefacto |
| Impacto público | dejar indicadores, protocolo y diseño de evaluación para futuras implementaciones | medir como requisito doctoral la reducción definitiva de pobreza, desigualdad o filtración |

La validación puede combinar revisión de expertos, Delphi, evaluación de criterios, estudio de caso, prueba piloto o comparación de escenarios. Los resultados esperados deben ser observables durante la tesis: completitud de fases, calidad de documentación, cumplimiento de requisitos de gobernanza, explicabilidad, equidad ex ante, utilidad percibida, reproducibilidad y capacidad de generar recomendaciones.

El caso de subsidios, ayudas o recursos sociales funcionará como escenario de demostración y validación del artefacto. No se presentará como prueba definitiva de impacto de una política pública. La metodología deberá incluir un plan de evaluación posterior, pero la tesis solo estará obligada a demostrar que ese plan es técnicamente y metodológicamente viable.

Esta delimitación protege la contribución doctoral: el objeto principal es el conocimiento metodológico y el artefacto de analytics; el caso público aporta evidencia de aplicabilidad, no una promesa de resultados sociales inmediatos.

## 10. Diseños metodológicos posibles

| Diseño | Ventaja | Riesgo |
|---|---|---|
| Design Science Research | permite construir y evaluar una metodología como artefacto | exige evaluación rigurosa del artefacto |
| Investigación basada en estudio de caso | facilita acceso a contexto real | puede limitar generalización |
| Investigación-acción | permite co-construir con una entidad | requiere acceso institucional sostenido |
| Métodos mixtos | integra evidencia técnica y percepción de actores | mayor complejidad |
| Revisión sistemática + Delphi | valida dimensiones y consenso experto | depende de expertos disponibles |

La combinación más recomendable es:

1. revisión sistemática y bibliométrica;
2. análisis comparativo de metodologías;
3. diseño del artefacto mediante Design Science Research;
4. co-diseño con actores públicos y sociales;
5. estudio de caso aplicado;
6. evaluación multicriterio y análisis de equidad.

## 11. Criterios de decisión

La idea debería avanzar a formulación doctoral si se confirman estos resultados:

- existen adaptaciones públicas, pero ninguna integra de forma completa ejecución, gobernanza, equidad, participación, operación e impacto;
- PRODIG8 tiene dimensiones reutilizables y una arquitectura que puede ampliarse sin perder coherencia;
- existe acceso a un caso real, datos o aliados institucionales;
- el artefacto puede evaluarse con indicadores reproducibles;
- la propuesta se articula explícitamente con una demanda territorial del proyecto BPIN;
- el cambio se presenta como extensión del proyecto aprobado y no como abandono del problema de asignación equitativa de recursos.

La idea debería reformularse o detenerse si:

- la búsqueda identifica una metodología pública equivalente ya validada para el mismo problema;
- no existe acceso a datos, funcionarios o escenario de validación;
- la metodología termina siendo una lista de buenas prácticas sin mecanismo de evaluación;
- se elimina la asignación equitativa de recursos y queda solo una metodología general;
- la propuesta no puede articularse con una demanda territorial habilitada.

## 12. Conclusión preliminar

La propuesta presenta **viabilidad científica preliminar alta, viabilidad metodológica alta y viabilidad administrativa condicionada exclusivamente por la Convocatoria 35 y sus instrumentos de ejecución**. La propuesta de admisión a la UNAL sirve como antecedente, pero no constituye por sí sola una restricción de la tesis.

La novedad no está en afirmar que el sector público necesita datos ni en aplicar CRISP-DM a una entidad. La posible contribución doctoral está en diseñar y validar una metodología que conecte:

- formulación del problema público;
- datos y capacidades institucionales;
- analítica predictiva y prescriptiva;
- equidad y derechos;
- gobernanza y responsabilidad;
- implementación;
- evaluación de impacto;
- aprendizaje y mejora continua.

La recomendación es continuar con la idea, delimitándola como una **adaptación de PRODIG8 para government analytics, validada mediante un caso público concreto**. La tesis debe evaluar el artefacto y su aplicabilidad; los efectos sociales y presupuestales de largo plazo deben quedar como evaluación futura o fase posterior de transferencia. La investigación del estado del arte debe continuar hasta cerrar una revisión sistemática y demostrar que la combinación propuesta no está ya resuelta por un marco existente.

## 13. Fuentes principales

1. OECD. (2019). *The Path to Becoming a Data-Driven Public Sector*. OECD Publishing. https://www.oecd.org/gov/the-path-to-becoming-a-data-driven-public-sector-059814a7-en.htm
2. OECD. (2019). *A Data-Driven Public Sector*. GOV/PGC/EGOV(2019)3. https://www.oecd.org/content/dam/oecd/en/publications/reports/2019/05/a-data-driven-public-sector_1c183670/09ab162c-en.pdf
3. World Bank. (2021). *Government Analytics: A Guide to Government Analytics*. https://www.worldbank.org/en/publication/government-analytics/a-guide-to-government-analytics
4. World Bank. (2021). *Artificial Intelligence in the Public Sector: Summary Note*. https://documents1.worldbank.org/curated/en/746721616045333426/pdf/Artificial-Intelligence-in-the-Public-Sector-Summary-Note.pdf
5. Straub, V. J., Morgan, D., Bright, J., & Margetts, H. (2022). *Artificial intelligence in government: Concepts, standards, and a unified framework*. arXiv:2210.17218. https://arxiv.org/abs/2210.17218
6. Batool, A., Zowghi, D., & Bano, M. (2023). *Responsible AI Governance: A Systematic Literature Review*. arXiv:2401.10896. https://arxiv.org/abs/2401.10896
7. Saltz, J. S., & Krasteva, I. (2022). Current approaches for executing big data science projects—A systematic literature review. *PeerJ Computer Science, 8*, e862. https://doi.org/10.7717/peerj-cs.862
8. Martinez, I., Viles, E., & Olaizola, I. G. (2021). Data science methodologies: Current challenges and future approaches. *Big Data Research, 24*, 100183.
9. Martinez-Plumed, F., et al. (2021). CRISP-DM Twenty Years Later: From Data Mining Processes to Data Science Trajectories. *IEEE Transactions on Knowledge and Data Engineering, 33*(8), 3048–3061. https://doi.org/10.1109/TKDE.2019.2962680
10. Studer, S., et al. (2021). Towards CRISP-ML(Q): A machine learning process model with quality assurance methodology. *Machine Learning and Knowledge Extraction, 3*(2), 392–413.
11. Huber, S., Wiemer, H., Schneider, D., & Ihlenfeldt, S. (2019). DMME: Data mining methodology for engineering applications—A holistic extension to the CRISP-DM model. *Procedia CIRP, 79*, 403–408. https://doi.org/10.1016/j.procir.2019.02.106
12. Ma, Z., Jørgensen, B. N., & Ma, Z. G. (2025). DataPro—A standardized data understanding and processing procedure. *Energy Informatics*. https://doi.org/10.1007/978-3-031-74738-0_10
13. Montoya-Murillo, D. A., Galvan-Cruz, S., Mora, M., & Andrade, E. L. M. (2025). A comprehensive review of heavyweight and lightweight SDLC for big data analytics systems. *IEEE Access, 13*, 101328–101367. https://doi.org/10.1109/ACCESS.2025.3577970
14. *Data-Driven Decision Making in the Public Sector: A Systematic Review*. (2022). IJAERS. https://ijaers.com/uploads/issue_files/21IJAERS-08202270-Data-Driven.pdf
15. *Big Data-Driven Public Policy Decisions: Transformation and Impact*. (2023). *SAGE Open*. https://doi.org/10.1177/21582440231215123
16. Velásquez, J. D., Gallego, L. J., & Cadavid, L. (2026). *Strategies for Executing Analytics Projects: Toward a Unified Framework of Methodologies* [manuscrito disponible en `idea-1/prodig8.docx`].
17. Universidad Autónoma de Manizales. (2026). *Términos de referencia para la selección de beneficiarios—Convocatoria 35 Eje Cafetero, BPIN 2024000100132*. https://www.autonoma.edu.co/sites/default/files/2026-02/terminos-de-referencia-conv-35-v3.pdf
18. Universidad Autónoma de Manizales. (2026). *Adenda No. 1 a los términos de referencia*. https://www.autonoma.edu.co/sites/default/files/2026-03/adenda-No-1-a-los-terminos-de-referencia-conv-35.pdf
19. Universidad Autónoma de Manizales. (2026). *Convocatoria 35 Eje Cafetero*. https://www.autonoma.edu.co/convocatoria-35-eje-cafetero

## 14. Próximas decisiones

1. Ejecutar una revisión sistemática PRISMA 2020 con una ecuación reproducible.
2. Construir una matriz comparativa de por lo menos 30 estudios y metodologías.
3. Identificar la demanda territorial exacta a la que se adscribirá la tesis.
4. Definir si el caso será subsidios de vivienda, recursos sociales, ayudas alimentarias o una comparación controlada.
5. Verificar la disponibilidad de datos y de una entidad pública para validar el artefacto.
6. Presentar al director una propuesta de una página, diferenciando problema, brecha, aporte, caso, validación y resultados medibles durante el doctorado.
7. Separar en la documentación de trabajo las restricciones de la convocatoria de la propuesta no vinculante presentada a la UNAL.
8. Solicitar concepto formal a la alianza únicamente sobre las obligaciones de la beca y la compatibilidad del nuevo alcance con el proyecto BPIN.
