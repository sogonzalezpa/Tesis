# Catálogo de fuentes de datos e inventario de problemas para validar PRODIG8-Público

**Ubicación:** `idea-1`  
**Fecha de corte:** 1 de octubre de 2026  
**Propósito:** identificar fuentes públicas reales y problemas analíticos que permitan construir un caso de validación retrospectiva de PRODIG8-Público sin depender de la adopción formal de la metodología por una entidad estatal.

## 1. Decisión metodológica

La tesis puede validarse con datos abiertos mediante un diseño de **backtesting temporal**:

1. construir el problema y el conjunto de datos usando información disponible hasta 2024;
2. producir predicciones, priorizaciones o asignaciones simuladas para 2025;
3. contrastar las estimaciones con los resultados observados en 2025;
4. comparar PRODIG8-Público con una línea base reproducible;
5. evaluar desempeño, equidad, trazabilidad, explicabilidad, robustez y utilidad para la decisión.

Este diseño demuestra que la metodología permite producir recomendaciones reproducibles y evaluables. No demuestra por sí solo que una política pública haya causado mejores resultados sociales.

## 2. Ficha mínima para catalogar cada fuente

Cada conjunto debe registrarse con los siguientes campos:

| Campo | Pregunta |
|---|---|
| Identificador | ¿Cuál es la URL, API, código Socrata o identificador del dataset? |
| Entidad productora | ¿Quién recoge, valida y publica la información? |
| Tema | ¿Pobreza, vivienda, salud, educación, movilidad, contratación, ambiente? |
| Unidad de análisis | ¿Persona, hogar, contrato, proyecto, institución, comuna, municipio, evento? |
| Cobertura geográfica | ¿Nacional, departamento, municipio, comuna, barrio o coordenada? |
| Cobertura temporal | ¿Qué años o fechas contiene? |
| Periodicidad | ¿Diaria, mensual, trimestral, anual o eventual? |
| Nivel de acceso | Abierto, agregado, anonimizado, restringido o no disponible |
| Formato | CSV, XLSX, JSON, API, SHP, GeoJSON, PDF |
| Metadatos | Definiciones, diccionario, licencia, responsable y fecha de actualización |
| Calidad | Completitud, consistencia, duplicados, faltantes y cambios de definición |
| Enlace | URL oficial y URL de documentación |
| Uso posible | Variable objetivo, predictores, restricción, línea base o validación |
| Riesgos | Sesgo, privacidad, discontinuidad, cambio metodológico o selección |
| Corte para backtesting | Fecha que separa entrenamiento y prueba |

## 3. Catálogo nacional de datos abiertos y metadatos

### 3.1 Portal de Datos Abiertos del Estado colombiano

**Fuente:** [datos.gov.co](https://www.datos.gov.co/)  
**Entidad coordinadora:** Ministerio de Tecnologías de la Información y las Comunicaciones, Gobierno Digital.

Es el catálogo central para localizar conjuntos de datos de entidades nacionales y territoriales. Publica fichas, responsables, fechas de actualización, formatos y, en muchos casos, APIs Socrata. La guía oficial de estandarización recomienda describir los conjuntos con metadatos y referencias compatibles con DCAT.

**Utilidad para PRODIG8:**

- inventariar fuentes antes de definir un proyecto;
- verificar disponibilidad, periodicidad y calidad;
- construir un catálogo de metadatos como producto de la fase de gobernanza;
- reproducir consultas mediante API.

**Riesgos:** que la existencia de un dataset en el catálogo no garantice continuidad, granularidad o calidad suficiente.

### 3.2 DANE: microdatos, metadatos e indicadores

**Fuentes:**

- [Catálogo Central de Datos y Microdatos](https://microdatos.dane.gov.co/)
- [Estadísticas por tema](https://www.dane.gov.co/index.php/estadisticas-por-tema)
- [Geoportal DANE](https://geoportal.dane.gov.co/)

**Temas útiles:**

- Gran Encuesta Integrada de Hogares;
- Encuesta Nacional de Calidad de Vida;
- Encuesta Nacional de Presupuestos de los Hogares;
- déficit de vivienda;
- pobreza monetaria y multidimensional;
- Censo Nacional de Población y Vivienda;
- educación, mercado laboral y demografía;
- estadísticas experimentales;
- cartografía y divisiones territoriales.

**Unidad:** persona, hogar, vivienda, municipio, departamento o área geográfica, según operación.

**Usos:** estimar vulnerabilidad, construir variables socioeconómicas, generar indicadores territoriales, evaluar cobertura y simular priorización.

**Restricciones:** muchos microdatos requieren registro o tienen anonimización; no deben combinarse para reidentificar personas u hogares.

### 3.3 DNP: TerriData, Mapa de Inversiones y sistemas territoriales

**Fuentes:**

- [TerriData](https://terridata.dnp.gov.co/)
- [Sistemas de información y datos abiertos del DNP](https://www.dnp.gov.co/LaEntidad_/Direccion-general/oficina-tecnologia-sistemas-informacion/Paginas/sistemas-de-informacion-y-datos-abiertos.aspx)
- Mapa de Inversiones;
- SISFUT;
- información de proyectos de inversión;
- MGA;
- indicadores de desempeño territorial;
- información de regalías y OCAD.

**Temas:** pobreza, finanzas territoriales, inversión, desempeño, servicios, población, salud, educación y proyectos.

**Usos:** relacionar necesidades territoriales con gasto, comparar municipios, evaluar priorización, construir restricciones presupuestales y hacer análisis espacial.

**Riesgos:** cambios en definiciones, diferencias entre información reportada y ejecutada, datos agregados y rezagos de publicación.

### 3.4 Sisbén IV y focalización social

**Fuente institucional:** [DNP—Sisbén IV](https://www.sisben.gov.co/)  
**Descripción metodológica:** [Sisbén IV](https://www.sdp.gov.co/gestion-estudios-estrategicos/sisben/metodologia-4)

Sisbén es una fuente clave para estudiar focalización, vulnerabilidad y errores de inclusión o exclusión. Sin embargo, la base individual no es un conjunto de datos abiertos irrestricto. Su uso requiere autorización, finalidad legítima, protección de datos y acuerdos de intercambio.

**Uso en la tesis:** puede utilizarse como marco conceptual, fuente agregada o futura fuente institucional condicionada. No debe asumirse como disponible para el caso abierto.

### 3.5 SECOP y contratación pública

**Fuentes:**

- [SECOP II—Contratos Electrónicos](https://www.datos.gov.co/Estad-sticas-Nacionales/SECOP-II-Contratos-Electr-nicos/jbjy-vk9h)
- [SECOP Integrado](https://www.datos.gov.co/Estad-sticas-Nacionales/SECOP-Integrado/rpmr-utcd)
- [Datos abiertos de Colombia Compra Eficiente](https://www.colombiacompra.gov.co/transparencia/datos-abiertos)

**Unidad:** proceso, contrato, proveedor, entidad, modalidad, cuantía, fecha y estado.

**Problemas analizables:**

- retrasos y modificaciones contractuales;
- concentración de proveedores;
- competencia y pluralidad de oferentes;
- riesgo de baja ejecución;
- distribución territorial de la contratación;
- predicción de procesos con probabilidad de incumplimiento;
- priorización de seguimiento.

**Ventajas:** alta granularidad, historial temporal y disponibilidad de API.

**Riesgos:** inconsistencias entre campos, contratos modificados, valores no comparables y ausencia de variables latentes sobre calidad real.

### 3.6 Sistema General de Regalías

**Fuentes:** DNP, Mapa de Inversiones, OCAD y datos publicados en datos.gov.co.

**Unidad:** proyecto, entidad territorial, sector, valor, fuente, fase, ejecutor, avance y producto.

**Problemas analizables:**

- priorización de proyectos;
- retrasos de ejecución;
- asignación territorial;
- riesgo de proyectos inconclusos;
- coherencia entre necesidades, inversión y resultados.

Es especialmente pertinente para la tesis por su relación con la convocatoria y el BPIN, pero debe distinguirse entre datos del programa de beca y datos de proyectos de inversión territorial.

### 3.7 Salud pública

**Fuentes:**

- [Datos abiertos del Ministerio de Salud](https://www.minsalud.gov.co/Paginas/datos-abiertos.aspx)
- SISPRO y cubos o reportes públicos;
- INS y vigilancia epidemiológica;
- datos territoriales de salud publicados en datos.gov.co.

**Unidad:** evento, municipio, institución, servicio, afiliación agregada o indicador.

**Problemas:** demanda de servicios, cobertura, mortalidad, oportunidad, distribución de recursos, vigilancia y priorización territorial.

**Riesgos:** datos personales, cambios de codificación, subregistro y restricciones de acceso.

### 3.8 Educación

**Fuentes:** Ministerio de Educación, SIMAT agregado, datos de matrícula, establecimientos, resultados y deserción disponibles en portales oficiales y datos.gov.co.

**Problemas:** riesgo de deserción, distribución de cupos, brechas territoriales, infraestructura, cobertura, transición a educación superior y asignación de apoyos.

**Riesgos:** datos de estudiantes generalmente protegidos; el caso debe trabajar con agregados o datos anonimizados.

### 3.9 Ambiente, clima y territorio

**Fuentes:**

- [Datos abiertos ICDE](https://datos.icde.gov.co/)
- IDEAM;
- Geoportal DANE;
- IGAC;
- autoridades ambientales;
- imágenes satelitales y datos geoespaciales públicos.

**Problemas:** riesgo de inundación, calidad del aire, deforestación, acceso a agua, vulnerabilidad climática, localización de infraestructura y priorización de intervenciones.

**Ventaja:** permite integrar analítica espacial y datos abiertos con cobertura temporal.

### 3.10 Medellín y Antioquia

**Fuentes:**

- [MEData](https://medata.gov.co/)
- [API de MEData](https://medata.app.medellin.gov.co/)
- GeoMedellín;
- datos abiertos de la Alcaldía de Medellín;
- Área Metropolitana del Valle de Aburrá;
- Gobernación de Antioquia;
- Metro de Medellín;
- [Datos abiertos del Metro](https://datosabiertos-metrodemedellin.opendata.arcgis.com/).

**Temas:** movilidad, seguridad, ambiente, espacio público, servicios, población, inversión, comunas, barrios y equipamientos.

**Problemas:** movilidad y congestión, ubicación de servicios, seguridad, riesgos territoriales, priorización de inversión y desigualdad intraurbana.

**Ventajas:** escala de comuna, barrio o coordenada; APIs y datos geográficos; pertinencia directa para Medellín.

### 3.11 Otras fuentes públicas complementarias

| Fuente | Posibles variables | Uso |
|---|---|---|
| ICBF | niñez, nutrición, protección | priorización de atención |
| Prosperidad Social | programas y transferencias agregadas | cobertura y focalización |
| Registraduría y Censo | población y participación, sujeto a disponibilidad | denominadores y contexto |
| Policía y Medicina Legal | seguridad y violencia agregada | riesgo territorial |
| Unidad para las Víctimas | desplazamiento y víctimas agregadas | vulnerabilidad y priorización |
| Superintendencias | vigilancia sectorial | riesgos regulatorios |
| Banco de la República | economía regional | contexto macroeconómico |
| IDEAM | clima y eventos | alertas y vulnerabilidad |
| Metro y transporte | viajes, afluencia, rutas | movilidad y accesibilidad |
| OpenStreetMap | vías, equipamientos y puntos de interés | análisis espacial y accesibilidad |

## 4. Inventario de problemas analíticos

El siguiente inventario cruza problemas públicos con fuentes, unidad de análisis y tipo de decisión.

| ID | Problema público | Fuentes posibles | Unidad | Analítica | Resultado verificable |
|---|---|---|---|---|---|
| P01 | Priorizar subsidios o ayudas para población vulnerable | DANE, TerriData, datos municipales, fuentes agregadas de Sisbén | comuna, barrio, municipio o hogar anonimizado | prescriptiva, optimización multiobjetivo | asignación simulada y comparación con 2025 |
| P02 | Detectar subcobertura y filtración territorial | DANE, TerriData, programas sociales agregados | territorio-programa | diagnóstico, equidad | mapas y métricas de cobertura |
| P03 | Priorizar inversión pública con restricciones presupuestales | Mapa de Inversiones, SGR, TerriData | proyecto-municipio | prescriptiva | cartera priorizada y escenarios |
| P04 | Predecir retrasos o incumplimientos contractuales | SECOP II, SECOP Integrado | contrato | predictiva y prescriptiva | ranking retrospectivo de riesgo |
| P05 | Detectar concentración de contratistas | SECOP | entidad-proveedor | descriptiva, redes y anomalías | indicadores de concentración |
| P06 | Priorizar mantenimiento de infraestructura | datos territoriales, movilidad, contratos, geodatos | activo o segmento | predictiva | riesgo y orden de intervención |
| P07 | Optimizar acceso territorial a servicios sociales | DANE, MEData, ICDE, equipamientos | hogar o zona | espacial y prescriptiva | cobertura potencial y brechas |
| P08 | Identificar zonas con riesgo de deserción educativa | MEN, DANE, TerriData | institución, municipio o zona | predictiva | backtesting de 2025 |
| P09 | Priorizar acciones de salud pública | MinSalud, INS, DANE | evento-territorio | predictiva y espacial | alerta o priorización |
| P10 | Optimizar respuesta ante emergencias climáticas | IDEAM, ICDE, alcaldías | territorio-evento | predictiva y prescriptiva | escenarios de recursos |
| P11 | Reducir desigualdad de acceso al transporte | Metro, Área Metropolitana, MEData, OSM | zona-ruta | espacial y optimización | accesibilidad simulada |
| P12 | Identificar zonas críticas de calidad del aire | SIATA, Área Metropolitana, IDEAM | estación-zona-tiempo | temporal y espacial | pronóstico y priorización |
| P13 | Priorizar alimentación y seguridad alimentaria | DANE, MEData, Banco de Alimentos, indicadores territoriales | zona-organización | prescriptiva | asignación simulada |
| P14 | Detectar riesgos de ejecución de proyectos SGR | Mapa de Inversiones, DNP | proyecto | predictiva | validación con estados observados |
| P15 | Localizar brechas de vivienda y servicios | DANE, ICDE, alcaldías | vivienda-zona | espacial y multicriterio | mapa de vulnerabilidad |
| P16 | Priorizar prevención de violencia | Policía, Medicina Legal, DANE, MEData | evento-zona-tiempo | espacio-temporal | evaluación retrospectiva |
| P17 | Mejorar focalización de apoyos a víctimas | Unidad para las Víctimas, DANE, TerriData | municipio-zona | equidad y asignación | cobertura potencial |
| P18 | Evaluar eficacia de programas públicos | DNP, SISFUT, TerriData, datos sectoriales | municipio-programa | evaluación y causalidad | indicadores comparables |
| P19 | Detectar duplicidades o inconsistencias de registros | datos.gov.co, SECOP, inversión | entidad-proyecto-persona anonimizada | calidad y anomalías | tasa de duplicados y reglas |
| P20 | Priorizar digitalización de trámites | datos de atención, solicitudes, tiempos y canales | trámite-entidad | descriptiva y optimización | cartera de automatización |

## 5. Problemas recomendados para un primer caso de tesis

### Opción A: asignación equitativa de recursos sociales

Es la opción más coherente con la trayectoria y la propuesta de la beca.

**Datos:** DANE, TerriData, MEData, indicadores de vulnerabilidad, datos geográficos y, si es posible, información agregada del Banco de Alimentos.

**Pregunta:** ¿Una metodología pública basada en PRODIG8 puede orientar una asignación más equitativa y trazable de recursos sociales que una regla territorial simple?

**Backtesting:** entrenar o calibrar con datos hasta 2024, simular asignaciones para 2025 y contrastar contra resultados observados.

**Riesgo:** sin asignación individual real, la comparación se limita a unidades territoriales e indicadores agregados.

### Opción B: riesgo de contratación pública

**Datos:** SECOP II y SECOP Integrado.

**Pregunta:** ¿Puede PRODIG8-Público estructurar de forma reproducible un proyecto para priorizar contratos con riesgo de retraso, modificación o baja ejecución?

**Ventaja:** datos abiertos, unidad contractual y resultados observables.

**Riesgo:** los resultados contractuales no siempre representan incumplimiento real ni calidad del servicio.

### Opción C: priorización de proyectos de inversión territorial

**Datos:** Mapa de Inversiones, SGR, TerriData y DANE.

**Pregunta:** ¿Puede una metodología de analítica prescriptiva apoyar la priorización equitativa de proyectos bajo restricciones presupuestales?

**Ventaja:** conexión directa con inversión pública y demandas territoriales.

**Riesgo:** resultados de proyectos pueden tener rezagos y cambios de administración.

### Opción D: accesibilidad a servicios y ayudas

**Datos:** MEData, ICDE, DANE, equipamientos, transporte y OpenStreetMap.

**Pregunta:** ¿Cómo priorizar nuevas ubicaciones o recursos para reducir desigualdades espaciales de acceso?

**Ventaja:** datos abiertos y validación geoespacial.

**Riesgo:** la accesibilidad calculada no equivale automáticamente al uso efectivo del servicio.

## 6. Criterios para seleccionar el problema final

Cada candidato debe calificarse de 0 a 3:

| Criterio | 0 | 1 | 2 | 3 |
|---|---:|---:|---:|---:|
| Datos abiertos disponibles | inexistentes | parciales | suficientes | completos y documentados |
| Horizonte temporal para backtesting | ninguno | un corte | dos cortes | serie suficiente |
| Resultado observable | ninguno | indirecto | agregado | directo |
| Pertinencia territorial | baja | general | Antioquia | Medellín/Antioquia y demanda explícita |
| Equidad medible | no | limitada | varias métricas | equidad central |
| Complejidad manejable | muy alta | alta | media | controlable |
| Reproducibilidad | baja | parcial | buena | alta |
| Alineación con PRODIG8 | débil | parcial | alta | directa |
| Riesgo de acceso | alto | medio-alto | medio | bajo |

Se recomienda avanzar con problemas que obtengan por lo menos 20 de 27 puntos y no tengan cero en datos, temporalidad o reproducibilidad.

## 7. Reglas de calidad y ética

- No intentar reidentificar personas, hogares o beneficiarios.
- No combinar fuentes para inferir datos personales protegidos.
- Documentar licencia, finalidad, responsable y fecha de descarga.
- Separar variables disponibles antes de la decisión de variables posteriores.
- No usar información de 2025 para construir predictores de una simulación de 2025.
- Registrar cambios de metodología y versiones de cada dataset.
- Reportar datos faltantes y sesgos de cobertura.
- Incluir revisión humana y explicación de las recomendaciones.
- Presentar la simulación como evidencia metodológica, no como impacto causal.
- Evitar que un ranking algorítmico se interprete como decisión automática sobre ciudadanos.

## 8. Recomendación de decisión

La mejor ruta inicial es construir un **catálogo de 10 a 15 datasets candidatos**, descargar sus metadatos y aplicar la matriz de puntuación. Después se debe elegir un único problema para el prototipo.

La prioridad recomendada es:

1. asignación equitativa de recursos sociales;
2. priorización de proyectos de inversión territorial;
3. riesgo de contratación pública;
4. accesibilidad territorial a servicios.

La primera opción conserva la continuidad temática con la propuesta de beca. La segunda y la tercera ofrecen mayor disponibilidad de resultados observables y pueden servir como casos alternativos si el acceso a datos sociales es insuficiente.

## 9. Fuentes oficiales consultadas

- [Datos Abiertos Colombia](https://www.datos.gov.co/)
- [MinTIC—Datos abiertos](https://gobiernodigital.mintic.gov.co/portal/Iniciativas/Datos-abiertos/)
- [Guía de estandarización de datos abiertos](https://herramientas.datos.gov.co/sites/default/files/Guia_Estandarizacion_DatosAbiertos_final.pdf)
- [DANE—Catálogo de microdatos y metadatos](https://microdatos.dane.gov.co/)
- [DANE—Estadísticas por tema](https://www.dane.gov.co/index.php/estadisticas-por-tema)
- [DNP—sistemas de información y datos abiertos](https://www.dnp.gov.co/LaEntidad_/Direccion-general/oficina-tecnologia-sistemas-informacion/Paginas/sistemas-de-informacion-y-datos-abiertos.aspx)
- [DNP—TerriData](https://terridata.dnp.gov.co/)
- [Sisbén IV](https://www.sisben.gov.co/)
- [Ministerio de Salud—Datos abiertos](https://www.minsalud.gov.co/Paginas/datos-abiertos.aspx)
- [Colombia Compra Eficiente—Datos abiertos](https://www.colombiacompra.gov.co/transparencia/datos-abiertos)
- [SECOP II—Contratos electrónicos](https://www.datos.gov.co/Estad-sticas-Nacionales/SECOP-II-Contratos-Electr-nicos/jbjy-vk9h)
- [SECOP Integrado](https://www.datos.gov.co/Estad-sticas-Nacionales/SECOP-Integrado/rpmr-utcd)
- [MEData](https://medata.gov.co/)
- [API de MEData](https://medata.app.medellin.gov.co/)
- [Datos abiertos del Metro de Medellín](https://datosabiertos-metrodemedellin.opendata.arcgis.com/)
- [Portal de datos abiertos ICDE](https://datos.icde.gov.co/)
- [DANE—Geoportal](https://geoportal.dane.gov.co/)

## 10. Próximos pasos

1. Crear una hoja de inventario con la ficha mínima para cada dataset.
2. Seleccionar datasets con cobertura 2024–2025.
3. Verificar APIs, diccionarios, licencias y frecuencia de actualización.
4. Construir tres problemas candidatos con variable objetivo, predictores y línea base.
5. Puntuar los problemas con la matriz de decisión.
6. Elegir un caso principal y uno alternativo.
7. Diseñar el protocolo de backtesting antes de descargar y modelar los datos de prueba.
