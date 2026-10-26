# WORLD HEROES — registro maestro permanente

Última actualización: **27/10/2026, Europe/Madrid**. Fuente de estado vigente del repositorio; leer junto con `AGENTS.md` antes de trabajar. Este archivo registra decisiones, implementación y evidencia; no sustituye la inspección del proyecto ni convierte una intención en una función terminada.

**Decisión definitiva vigente:** las cuatro pantallas grandes independientes están **RECHAZADAS**, no aprobadas. Solo se permite el panel compacto original con **cuatro botones inferiores: Información, Equipo, Habilidades y Evolución**. Cambian el contenido del mismo marco y comparten un solo visor 3D. Los botones superiores duplicados quedan desactivados y fuera de navegación. No reconstruir ni reactivar las ventanas grandes desde herramientas históricas; sus PNG, scripts y referencias se conservan sin borrar. No avanzar a Match-3 hasta revisar panel/personajes.

## Estados y mantenimiento

| Estado | Significado |
| --- | --- |
| COMPLETADO | Entrega o implementación realizada en el alcance indicado; debe indicar su verificación y límites. |
| COMPROBADO | Existe evidencia concreta de inspección o prueba, con fecha y alcance. No implica aceptación artística ni producto completo. |
| EN CURSO | Trabajo iniciado y todavía sin cerrar; anotar qué falta. |
| PENDIENTE | Trabajo no realizado o sin comprobación suficiente. |
| BLOQUEADO | No puede activarse o completarse por una dependencia identificada; indicar qué falta. |

Actualizar al finalizar cada encargo importante: fecha, estado real, decisiones nuevas, pruebas, límites, última tarea y siguiente paso. Actualizar las secciones existentes sin duplicarlas; añadir al historial solamente decisiones y cambios importantes. Mantener el alcance aprobado aunque una parte siga pendiente. No borrar decisiones anteriores: indicar cuál las sustituye y por qué. Distinguir siempre prueba aislada, ejecución principal, inspección de archivos y aceptación visual del usuario.

## 1. Objetivo comercial y características generales

**Objetivo aprobado:** desarrollar World Heroes como juego comercial de fantasía épica, con acabado profesional, identidad azul y dorada, cinco héroes 3D, Aeryx, aldea y combate Match-3, progresión y campaña de **siete mundos**. Prioridades: máxima automatización, simplicidad, calidad visual, coherencia y conservación del trabajo aprobado.

**COMPROBADO:** proyecto Unity 6, versión `6000.6.4f1`; URP, TextMeshPro y nuevo Input System. Village y la presentación de Héroes son la base existente. El estado actual no constituye un juego comercial terminado.

**PENDIENTE de recuperar o definir con evidencia:** plataformas comerciales, monetización, público, precios, calendario de lanzamiento, condiciones de distribución y documentación detallada de los siete mundos. No se deduce una plataforma ni un modelo de negocio a partir del nombre del juego.

## 2. Decisiones y reglas aprobadas

1. Conservar todo el trabajo existente. No borrar ni reemplazar escenas, scripts, modelos, armas, animaciones o imágenes válidos sin autorización. Inspeccionar código y referencias antes de modificar; respaldar cambios importantes.
2. Reutilizar sistemas, prefabs, clips y configuraciones compatibles. No reconstruir el panel principal de Héroes ni duplicar héroes, armas activas, paneles o botones. Dos dagas de Shadows son una configuración solicitada, no dos personajes.
3. Mantener Unity 6, estética fantástica azul/dorada y los cinco héroes originales. No usar Blender ni modificar destructivamente FBX/Tripo. No gastar créditos ni generar personajes nuevos sin autorización.
4. Solicitar autorización para cambios adicionales ajenos al encargo y decisiones importantes o irreversibles. Continuar autónomamente con el trabajo ya autorizado y reversible. No simular resultados ni afirmar comprobaciones inexistentes.
5. Conservar los cuatro PNG históricos, dragón Aeryx, marcos y adornos como recursos. Las cuatro pantallas grandes están rechazadas; conservar sus PNG no autoriza reactivarlas. Originales intactos, mejora IA real con Upscayl `digital-art-4x`, salida 3840 × 2160, proporciones conservadas y alfa real. No inventar transparencias ni eliminar los interiores azules. No instalar herramientas adicionales sin explicarlas previamente.
6. Información y Equipo conservan su alfa. Habilidades y Evolución retiran únicamente el negro previsto como ventana transparente. Evitar halos; comprobar visualmente. El adorno inferior no debe tapar Vida/XP. Los datos variables pertenecen a Unity/TMP, nunca a nuevos textos pintados en PNG.
7. **Vigente desde el rediseño prioritario:** Información, Equipo, Habilidades y Evolución se abren exclusivamente con los cuatro botones inferiores del panel compacto original. Los superiores duplicados se desactivan. Cambia solo el contenido derecho; se conservan cinco retratos, un visor 3D, selección, animación, barras compartidas y Aeryx. No duplicar estadísticas, modelos o controles. El único cierre del panel devuelve a Village. La navegación anterior por cuatro ventanas y flechas Volver queda sustituida; sus assets se conservan fuera de la navegación activa.
8. Interfaz 16:9, incluida 1080p y 4K; sin deformar, con efectos suaves azules. Mismo modelo real, giro de ratón y animaciones existentes.
9. Presentación vigente: un mismo visor sobre la plataforma original en todas las pestañas, con giro de ratón. Kaeldor conserva su modelo y postura aceptables. Corregir huesos, muñecas, agarres y apoyo reales; no considerar resuelta una pose por mover cámara o compilar. Revisar frente, laterales, espalda y animación. Se reutilizan imágenes, marcos, insignias, barras, botones, retratos y tipografía aprobados. Las cámaras y fondos locales independientes del encargo anterior ya no forman la presentación activa.
10. Estadísticas, inventario y recursos reales y sincronizados. Cero confirmado se muestra como `0`; valores todavía desconocidos quedan **en blanco**, sin «Sin definir» ni guiones. No mostrar el perfil provisional de otros héroes como atributos confirmados. Ranuras visuales sin texto «Vacío». Acciones de equipo/mejora solamente cuando haya contenido y operación real. No inventar objetos, habilidades, costes, evoluciones, modelos ni recursos.
11. Vida inicial llena y XP vacía al nivel 1. Daño reduce vida; XP aumenta y sube niveles automáticamente, gratis y sin curación implícita. Evolución especial es un sistema diferente que consume recursos ganados jugando cuando sus reglas existan.
12. Seis estadísticas requeridas: Ataque, Defensa, Velocidad, Crítico, Resistencia y Precisión; además vida, XP y maná/recurso de clase cuando exista. Respetar los hitos de vida ya definidos.
13. Habilidades: cinco por héroe, selección de icono central y **nombre dinámico inmediatamente debajo**, descripción, nivel 1–20, daño/efecto, recarga, costes oro/cristales y Mejora validada. Equipo: ranuras, Equipar/Mejorar/Quitar reales. Evolución: nombre/rango, niveles actual/siguiente, seis estadísticas actuales/futuras y requisitos reales.
14. Armas originales en sus manos, acompañando la animación; ajustar individualmente agarre y dedos. Kaeldor se conserva. Thorgrim es prioridad: hombro/brazo/codo/antebrazo/muñeca naturales, brazo derecho sin desplazamiento trasero, mano cerrada en el mango y pies apoyados durante Idle/animaciones. Pose T solo como referencia. Altherion necesita bastón **más largo y fino mediante proporciones no uniformes**, no la reducción uniforme anterior. Lyriana debe sostener el arco con brazos naturales. Shadows debe usar el original aprobado con rostro visible y dos dagas agarradas por empuñaduras, nunca hojas. Sin Blender ni modelos nuevos.
15. Orden aprobado del encargo amplio: paneles → Kaeldor/Thorgrim → Altherion/Shadows/Lyriana → contadores. No repetir tareas ya resueltas. Actualizar este registro después de entregas importantes y dar informe breve en español.

## 3. Héroes, Aeryx, enemigos y siete mundos

| Personaje | Rol aprobado | Modelo/arma vigente | Estado real |
| --- | --- | --- | --- |
| Kaeldor | Guerrero | Original `Kaeldor/kaeldor.fbx`; espada `Espada_Kaeldor_1`, derecha | COMPROBADO: 3D, reposo, giro y anclaje; contacto fino de dedos PENDIENTE. |
| Thorgrim | Enano guerrero | Original `thorgrim/thorgrim.fbx` mediante `Thorgrim_Reusable`; martillo izquierdo | COMPROBADO en revisión compacta: corrección de cadenas de brazos después del Idle, muñeca/knuckles alineados al mango, Grip centrado en el mango y apoyo medido durante animación. Altura de presentación 3 frente a 3,6 de referencia humana; profundidad proyectada sobre la plataforma. Aceptación artística del usuario PENDIENTE. |
| Altherion | Mago | Original `Altherion_1/Altherion_1.fbx`; bastón derecho | COMPROBADO: brazo doblado, muñeca de agarre, bastón +40 % de longitud y −28 % de grosor respecto al estado anterior, con escala no uniforme e inclinación natural para no tapar la placa del nombre. FBX intacto. |
| Shadows | Asesino | Original `fantasy_armored_warrior_3d_model/...fbx`, con rostro; dos dagas | COMPROBADO: rostro visible en los renders actuales, dos manos en empuñaduras, Grip corregido hacia centro del mango y muñecas orientadas para sujetarlo. No se ha creado un modelo nuevo. |
| Lyriana | Arquera | Original `Lyriana/Lyriana.fbx`; arco izquierdo | COMPROBADO: hombro/codo/antebrazo y muñeca de agarre corregidos en Idle; dedos rodean el mango original del arco. |
| Aeryx | Compañero de Kaeldor | `AeryxRiggedOriginal` / `AeryxOriginalCompanion.prefab` | COMPROBADO históricamente: solo con Kaeldor, cuatro apoyos, respiración/cabeza y giro independiente. En el panel compacto vigente se conserva su 3D junto a Kaeldor; la ocultaci?n por PNG corresponde ?nicamente al dise?o grande rechazado. |

**Aeryx:** el rig original tiene 51 huesos de skin, sin clips importados ni controles independientes de alas/cola/párpados. El reposo procedimental no equivale a vuelo o ataque. Estos estados siguen PENDIENTES; al introducir clips, evitar dos animadores escribiendo sobre los mismos huesos.

**Enemigos — PENDIENTE:** no hay roster ni reparto definitivo por mundo documentado en esta copia. Se encontraron en la caché local paquetes de criaturas: LowPoly Fantasy Monsters Pack Ver1.0 DEMO (rutas de troll, hobgoblin y zombie), Monstr1, Dragon PBR, Wolf y Wild Boar. Su existencia está COMPROBADA por inventario del paquete; ninguno está importado por sus rutas originales ni conectado a combate. Son candidatos disponibles, no enemigos aprobados ni contenido integrado. No confundir Dragon PBR con Aeryx ni sustituirlo.

| Mundo del alcance de siete | Evidencia disponible | Estado |
| --- | --- | --- |
| 1 | Existe `Assets/Scenes/World1_Level1.unity`; el nombre no acredita nivel jugable ni identifica el mundo aprobado. | PENDIENTE de auditar y recuperar nombre/temática/reglas. |
| 2 | Sin ficha identificada en la documentación revisada. | PENDIENTE de recuperar decisiones aprobadas. |
| 3 | Sin ficha identificada en la documentación revisada. | PENDIENTE de recuperar decisiones aprobadas. |
| 4 | Sin ficha identificada en la documentación revisada. | PENDIENTE de recuperar decisiones aprobadas. |
| 5 | Sin ficha identificada en la documentación revisada. | PENDIENTE de recuperar decisiones aprobadas. |
| 6 | Sin ficha identificada en la documentación revisada. | PENDIENTE de recuperar decisiones aprobadas. |
| 7 | Sin ficha identificada en la documentación revisada. | PENDIENTE de recuperar decisiones aprobadas. |

No se han reducido los siete mundos a uno. Faltan nombres, ambientaciones, enemigos, jefes, cantidad de niveles y desbloqueos documentados: recuperar la fuente previa antes de inventar o implementar contenido.

## 4. Panel compacto y cuatro pestañas: estado real

**COMPLETADO y COMPROBADO en Play aislado y editor principal:** `HeroMenuV2` y `HeroRightScreens` reutilizan exclusivamente cuatro botones inferiores, en orden Información/Equipo/Habilidades/Evolución, con marcos e iconos originales y rótulos TMP. La quinta acción antigua y los cuatro botones superiores quedan inactivos. Cambia solo el contenido derecho; mismo modelo, selección y cámara. Vida/XP/nivel se comparten una sola vez en la franja superior derecha liberada, sin tapar la navegación inferior. Cerrar reutiliza el botón existente. Los PNG históricos permanecen intactos como recursos, sin aprobación para reconstruir pantallas grandes.

**COMPROBADO el 27/10/2026:** 173 comprobaciones superadas, cero fallos, en Unity 6000.6.4f1 aislado. Raycasts y clics de cuatro botones × cinco héroes, orden inferior, controles superiores inactivos, instancia compartida y datos/contexto. Capturas 1080p/4K en `Validation/FooterNavigation_20261027`. También se refrescó y reinició Play del editor principal: clics nativos en los cuatro botones muestran sus secciones dentro del mismo marco, con iluminación azul y héroe conservado. El arma original visible se identifica en Equipo, incluidas ambas dagas de Shadows, sin conceder inventario ni bonos ficticios. `Preservation.json` comprueba 278 archivos Tripo, Kaeldor, escena guardada y partida intactos, y scripts idénticos a la copia probada. Copia previa: `Backups/FooterNavigation_20261027`.

**PENDIENTE:** aceptación/revisión artística de Thorgrim, Shadows, Altherion y Lyriana. Esta entrega no cambia sus poses ni la postura aprobada de Kaeldor. Evolución, habilidades y acciones de equipo siguen dependiendo de sus reglas/datos reales; no se simulan resultados. Al salir de la sesión antigua tras recargar scripts apareció una excepción `IndexOutOfRangeException` de Unity UI `Selectable` durante restauración del editor; la nueva entrada en Play permitió probar navegación. Investigar si se reproduce; no se han borrado cachés ni sustituido la escena.

| Panel | Implementación y comprobación | Pendientes/dependencias |
| --- | --- | --- |
| Información | Seis campos dentro del marco original; se muestran atributos confirmados o blanco, sin «Sin definir». Mismo visor y HUD compartido. | Estadísticas adicionales y balance definitivo de cuatro héroes. |
| Equipo | Ocho ranuras visuales conservando IDs, sin «Vacío». Equipar/cambiar/quitar contextuales para piezas poseídas y compatibles; estadísticas del mismo store. | Catálogo de producción y mejora real de objetos; no se muestran acciones ficticias. |
| Habilidades | Cinco iconos, selección central, nombre TMP debajo y descripción/nivel/efecto/recarga/coste dinámicos si están configurados. Confirmación y mejora contextual reales; campos ausentes en blanco. Mismo visor fuera del área de contenido. | Nombres, efectos, costes, desbloqueos y recargas reales de las 25 habilidades. |
| Evolución | Pestaña del mismo panel; muestra indisponibilidad sin inventar rango/requisitos/estadísticas futuras ni botones de gasto. | `IHeroEvolutionSource` real y reglas/modelos aprobados; no confundir con XP gratuita. |

Las pruebas con datos TEST verifican operaciones, no conceden equipo o recursos al jugador ni demuestran contenido definitivo. El castillo visible proviene del gráfico aprobado existente; Village 3D sigue siendo geometría de prototipo. El fondo local nuevo despeja exclusivamente el retrato; no reemplaza la aldea.

**Evidencia vigente:** `Validation/CompactRevision/Checks.txt`, `Unity.log`, `Screens`, `Hands` y `Preservation.json`. Pruebas en Play de Unity 6000.6.4f1 en copia aislada: cuatro pestañas × cinco héroes, misma instancia de visor, ocho ranuras, controles contextuales, transacciones con TEST exclusivamente aislado, estadísticas efectivas, nombre/coste/recarga dinámicos, vida/XP compartidas, ratón Input System, brazo derecho de Thorgrim y apoyo durante animación. Renders 1080p, cuatro pestañas a 4K, frente/±45°/lateral/espalda de cinco héroes y seis agarres cercanos. No se presenta esto como aceptación artística final del usuario ni prueba manual nueva en el editor principal. Evidencias históricas de los PNG y pantallas anteriores permanecen en `Validation/ApprovedPanels`, `PanelFraming_20261026` y `DamageAnimation_20261026`.

## 5. Modelos, armas, rigging y animaciones

**COMPROBADO:** se conservan FBX, materiales y texturas originales. Los rigs de producción son Generic, sin certificar Humanoid de producción. Anclajes `Grip`/`HeroWeaponSocket` siguen la palma; poses locales de cierre sobreviven al reposo. Esto no certifica contacto artístico perfecto de cada dedo con cada empuñadura.

Reposos usados: Kaeldor `wait (1)`/estado `wait`; Thorgrim clip `idle.001`/estado `idle_001`; otros tres `Altherion_PanelIdle`, `Lyriana_PanelIdle`, `Shadows_PanelIdle`, adaptados sobre sus propios rigs. Se conservan controladores y correcciones de brazos aprobadas, con aplicación después del Animator cuando corresponde. No se ha forzado una animación de espada a arco/bastón.

Thorgrim: el objeto de escena `reposo` no tenía renderizadores y su binding estaba vacío. Se reutiliza el prefab existente del FBX original con `HeroApprovedIdlePose`; se conservan los objetos vacíos y los valores aprobados. Shadows: el original faltaba en disco y se recuperó mediante copia desde la Papelera; no se generó un sustituto. El montaje usa dos instancias del recurso de daga original, una por mano.

**COMPROBADO solo como ensayo aislado:** retargeting Humanoid Kaeldor → Thorgrim para reposo y caminar, Avatars válidos y reproducción real. `Assets/RetargetingTrial` y `Validation/RetargetingTrial` conservan pruebas. Apoyo, deslizamiento y diferencias de postura no tienen aprobación artística final; no migrar producción por el mero hecho de que `Avatar.isValid` sea verdadero.

**COMPROBADO en la corrección vigente:** `HeroNaturalIdlePose` aplica IK de brazos solo en estados Idle, después de las correcciones existentes y antes de dedos/medición. Ajusta también orientación real de muñecas para que la línea de nudillos corresponda al mango; conserva orientación de armas y coincidencia Grip/palma. Se han corregido los puntos de agarre de martillo y dagas y la posición de palma de arco/bastón en prefabs derivados. No cambia longitudes de huesos, pesos ni mallas. Kaeldor queda excluido de la corrección nueva. `HeroModelPreview` mide apoyo después de pose/agarre; Thorgrim conserva ancla de suelas y proyecta profundidad coherente con la plataforma. Las correcciones previas se conservan; no se reemplaza el rig por Humanoid. La prueba anterior que giraba todas las armas para alinearlas con nudillos se mantiene descartada: la solución vigente orienta la muñeca para sujetar el arma, no tumba el arco.

**PENDIENTE:** aceptación visual del usuario y evaluación artística exhaustiva de contactos de dedos/ropa en todas las futuras animaciones, además de los estados completos de juego. No atribuir a las comprobaciones de anclaje una corrección de pesos de skin o de todas las intersecciones posibles.

## 6. Paquetes encontrados, importados y pendientes

Auditoría de 26/10/2026: caché `%APPDATA%/Unity/Asset Store-5.x`, lectura de manifiestos internos sin importar ni ejecutar paquetes. Ninguno de estos once paquetes tiene archivos presentes en sus rutas originales de Assets. La ausencia por ruta no certifica que no exista alguna copia renombrada; no se encontró evidencia de integración. No se publican paquetes de terceros ni se da por comprobada su licencia/distribución comercial.

| Paquete descargado | Uso candidato | Estado |
| --- | --- | --- |
| Kevin Iglesias — Human Basic Motions FREE | Reposo y movimiento humanos | COMPROBADO descargado; importación/compatibilidad/integración PENDIENTES. |
| Kevin Iglesias — Human Melee Animations FREE | Guerrero y posibles dagas compatibles | COMPROBADO descargado; integración PENDIENTE; revisar agarres individualmente. |
| Kevin Iglesias — Dwarf Melee Animations FREE | Thorgrim y martillo | COMPROBADO descargado; integración PENDIENTE; preservar brazos aprobados. |
| Kevin Iglesias — Human Archer Animations FREE | Lyriana/arco | COMPROBADO descargado; integración PENDIENTE. |
| Kevin Iglesias — Human Spellcasting Animations FREE | Altherion/bastón y magia | COMPROBADO descargado; integración PENDIENTE. |
| DoubleL — RPGAnimationsPackFREE | Acciones RPG y variantes de combate | COMPROBADO descargado; selección y compatibilidad PENDIENTES. |
| LowPoly Fantasy Monsters Pack Ver10DEMO | Criaturas y animaciones candidatas | COMPROBADO descargado; importación/aprobación PENDIENTES. |
| Monstr1 | Criatura y acciones candidatas | COMPROBADO descargado; importación/aprobación PENDIENTES. |
| Dragon PBR | Dragón candidato, separado de Aeryx | COMPROBADO descargado; importación/aprobación PENDIENTES. |
| Realistic Furry Wolf FREE sample REALISTIC FOREST ANIMALS | Lobo candidato | COMPROBADO descargado; importación/aprobación PENDIENTES. |
| WIld Boar - Free sample Ultrarealistic Forest Animals | Jabalí candidato | COMPROBADO descargado; importación/aprobación PENDIENTES. |

**Importado y utilizado:** FBX originales Tripo, clips/controladores propios de Kaeldor y Thorgrim, tres reposos adaptados de presentación y copias Humanoid de ensayo. No atribuir estos reposos a los paquetes recién inventariados. No se importó ningún paquete durante este encargo documental.

## 7. Estados de animación necesarios

| Estado requerido | Situación |
| --- | --- |
| Reposo | COMPROBADO en presentación compacta de cinco héroes, con corrección natural de brazos/agarres para cuatro y Kaeldor conservado; Aeryx procedimental. Reposo de combate por clase PENDIENTE. |
| Movimiento | COMPROBADO caminar Kaeldor/Thorgrim únicamente en ensayo Humanoid. Movimiento de producción de todos PENDIENTE. |
| Ataque | PENDIENTE por arma y clase, con agarres, tiempos y eventos válidos. |
| Habilidad | PENDIENTE por habilidad aprobada y efectos correspondientes. |
| Defensa | PENDIENTE de reglas, clips y transiciones. |
| Daño | COMPLETADO y COMPROBADO para Kaeldor y Thorgrim: clip original Generic `hit_to_stomach` y adaptación por deltas de rotación sobre el rig propio de Thorgrim. `HeroMenuV2.ReceiveDamage` lo activa únicamente cuando baja la vida y ambos regresan al reposo original. PENDIENTE para los otros tres héroes y conexión al futuro motor Match-3. |
| Victoria | PENDIENTE de selección de clip y conexión al resultado. |
| Derrota | PENDIENTE de clip, transición y reglas de resultado. |

Inventariar clips de cada paquete, rig, Avatar, variantes de arma, root motion, duración, bucles y eventos antes de elegir. No afirmar que un estado está disponible solo por el nombre comercial del paquete. Reutilizar cuando la compatibilidad y el resultado visual estén comprobados.

## 8. Conexión con combate Match-3

**COMPLETADO/COMPROBADO como contrato de datos:** `HeroProgressStore` implementa `IHeroCombatSource.TryCaptureCombatant`; entrega las mismas estadísticas efectivas y habilidades que usa la UI. Esto no implementa un motor de combate.

**PENDIENTE y detenido por prioridad del usuario:** tablero, turnos, reglas de combinaciones, objetivos, daño, recarga, selección de enemigos, premios y resultado. **No avanzar a Match-3 antes de corregir y revisar panel/personajes.** No se ha encontrado un motor Match-3 funcional en los scripts revisados. La existencia de `World1_Level1.unity` no cambia esta conclusión.

**BLOQUEADO para conexión definitiva:** faltan reglas de combate y contenido confirmado. Una vez definidos, enlazar reposo/movimiento/ataque/habilidad/defensa/daño/victoria/derrota con eventos reales del combate, resolver los efectos una sola vez y enviar resultados al almacén compartido. No mantener estadísticas, carteras o XP paralelas, ni usar animaciones como prueba de combate terminado.

## 9. Recursos, estadísticas, XP, evolución, inventario y habilidades

- **COMPROBADO — fuente única:** `HeroProgressStore.Shared`, persistencia `Application.persistentDataPath/world-heroes-v2.json`, lectura efectiva de base + nivel + mejoras configuradas + equipo. Eventos comunes actualizan menú y subpaneles. No incorporar el guardado real a Git.
- **COMPROBADO — transacciones:** pruebas aisladas de equipar/quitar, mejoras con confirmación, costes exactos, rechazo de doble operación, máximos y persistencia. Las pruebas históricas más amplias están en `Validation/HeroesConnected`; no confundir sus fixtures con datos de producción.
- **BLOQUEADO — recursos jugables:** madera, oro, metal y cristales existen como contrato, pero la partida real tiene `resourcesKnown = false`. Sus valores quedan en blanco. No inicializar saldos de ejemplo. Cero confirmado se muestra como `0` y cambia por evento real.
- **COMPROBADO — Kaeldor:** nivel inicial 1; vida base 100, ataque 25, defensa 20, velocidad 15, poder 30. Hitos de vida máxima base 1→100, 10→110, 20→120. Tabla existente de XP 100, 200, …, 1900 para niveles 1→20; no extrapolar después del límite.
- **COMPROBADO — otros cuatro:** perfil compartido `ProvisionalInitialStats.asset` y progreso existente se conservan, sin sobrescribir datos guardados. No es balance definitivo; la interfaz compacta deja en blanco los atributos no confirmados, en lugar de presentar el baseline provisional como estadísticas aprobadas. **PENDIENTE** aprobar atributos individuales.
- **PENDIENTE — adicionales:** crítico, resistencia, precisión y maná/recurso de clase carecen de valores aprobados y quedan en blanco; maná no se muestra como barra inventada. No transformar campos internos cero en cifras reales.
- **COMPROBADO — vida/XP:** mismo estado en todas las pantallas, daño/curación explícitos, XP gratuita automática, vida actual conservada al subir nivel y hitos comprobados. El combate todavía no concede premios reales.
- **COMPLETADO como operaciones, BLOQUEADO por contenido — inventario:** equipamiento real por ID, compatibilidad, propiedad y estadísticas efectivas sin acumular bonos al releer. Ocho ranuras visuales; los seis IDs originales se preservan y Gloves/OffHand se añaden al final. No hay catálogo jugable aprobado ni objetos concedidos al jugador. Mejorar equipo requiere proveedor real.
- **COMPLETADO como estructura, BLOQUEADO por contenido — habilidades:** 25 IDs estables, cinco por héroe; selección/nombre/icono, rangos hasta 20, requisitos y confirmación. Assets con `skillConfigured = false`, sin efectos/costes finales. No activar con datos ficticios.
- **PENDIENTE — evolución especial:** `IHeroEvolutionSource` y comparación preparados; no hay proveedor definitivo, rangos, costes o modelos aprobados. No confundir con las mejoras individuales de atributos heredadas (`attributeUpgrades`) ni con nivel gratuito por XP. Nunca inventar una evolución o gastar recursos sin regla real.

## 10. Errores conocidos, pendientes y prioridades

**Incidencia del editor observada el 27/10:** al salir de la sesi?n antigua despu?s de recargar scripts apareci? `IndexOutOfRangeException` de Unity UI `Selectable` al restaurar objetos del editor. La nueva entrada en Play y las pruebas de navegaci?n funcionaron; no se atribuye a un fallo resuelto ni se han borrado cach?s/escena. Investigar si se reproduce.


| Prioridad | Tarea o incidencia | Estado y dependencia |
| --- | --- | --- |
| 1 | Aceptación visual del panel compacto y de los cinco héroes corregidos, particularmente Thorgrim, apoyo y agarres | COMPROBADO en Play aislado y renders; aceptación artística del usuario PENDIENTE. No reactivar ventanas grandes ni avanzar a Match-3. |
| 2 | Recuperar diseño comercial, fichas de los siete mundos y roster de enemigos desde fuentes previas | PENDIENTE; faltan documentos verificables. No recortar el alcance. |
| 3 | Auditar paquetes descargados y probar primero Kaeldor/Thorgrim en aislamiento, después mago/asesino/arquera | PENDIENTE; revisar compatibilidad y derechos antes de integrar/distribuir. |
| 4 | Confirmar atributos por héroe, las 25 habilidades, objetos, recursos y evoluciones | PENDIENTE; activación de acciones BLOQUEADA hasta tener datos reales. |
| 5 | Implementar economía y combate Match-3 conectados al store y estados de animación | PENDIENTE; depende de reglas/contenido. |
| Técnica | Excepción interna de inicio `UnityEditor.Search.SearchDatabase` en algunas pruebas | COMPROBADO en logs; no impidió las pruebas de panel. PENDIENTE de diagnóstico específico; no borrar cachés a ciegas. |
| Técnica | Avisos históricos de scripts ausentes en `Ficha_Kaeldor`, uGUI Selectable en recargas anteriores y APIs de editor obsoletas | Históricos documentados; vigencia actual PENDIENTE de auditoría específica. No atribuirlos a errores nuevos de los paneles. |
| Técnica | Sufijo `i` de la tabla hexadecimal de XP | COMPROBADO y aclarado mediante carga y reserialización real en Unity 6000.6.4f1: Unity conserva el sufijo y los mismos 19 enteros 100…1900. La sospecha anterior de corrupción no se confirmó; no retirar el marcador ni alterar los valores. Evidencia en `Validation/DamageAnimation_20261026/Setup.txt`. |
| Recuperación | `Assets/_Recovery/0.unity` | COMPROBADO anteriormente idéntico a la escena previa de Village. Conservado; no restaurar sobre el trabajo vigente sin comparar. |
| Portabilidad | Tripo Bridge en `Packages/manifest.json` usa una ruta local de Descargas | COMPROBADO. PENDIENTE hacer portable en un encargo apropiado; no publicar credenciales ni asumir que otro equipo puede resolver esa ruta. |
| Git | Muchos cambios de Unity y archivos nuevos siguen fuera del commit documental | COMPROBADO. PENDIENTE revisar dependencias, licencias, tamaño y datos sensibles antes de sincronizar el proyecto completo. |

**EN CURSO:** no hay una integración de combate o animaciones en ejecución al cerrar este encargo; la siguiente fase aún no se ha iniciado. Este registro no autoriza cambios adicionales por sí solo.

## 11. Archivos y puntos de entrada importantes

| Ruta | Función |
| --- | --- |
| `AGENTS.md` | Reglas permanentes y lectura/actualización obligatoria de este registro. |
| `Assets/Scenes/village.unity` | Escena principal de integración; conservar `Panel_Heroes` y sus conexiones. |
| `Assets/Scenes/World1_Level1.unity` | Escena existente; jugabilidad pendiente de auditar. |
| `Assets/Scenes/village 1.unity`, `SampleScene.unity` | Escenas existentes conservadas, no sustituir Village por ellas. |
| `Assets/Prefabs/Panel_Heroes.prefab` | Prefab existente conservado. |
| `Assets/WorldHeroesV2/Prefabs/` | Prefabs de menú, compañero original y `ApprovedPanelBack.prefab`. |
| `Assets/WorldHeroesV2/Reusable/Heroes/`, `Reusable/Weapons/` | Héroes y armas originales reutilizables con anclajes. |
| `Assets/WorldHeroesV2/Presentation/` | Modelos/prefabs de presentación y reposos adaptados. |
| `Assets/TripoModels/` | Modelos/materiales/texturas fuente protegidos. |
| `Assets/WorldHeroesV2/Data/` | Cinco héroes, Aeryx, perfil provisional y configuración existente. |
| `Assets/WorldHeroesV2/Runtime/HeroMenuV2.cs`, `HeroLargePanels.cs`, `HeroLargePanelView.cs` | Selección, navegación y datos de pantallas grandes. |
| `HeroModelPreview.cs`, `HeroPreviewGeometry.cs`, `HeroPreviewDrag.cs`, `HeroPortraitBackdrop.cs` en Runtime | Cámara/encuadres, medición, giro y fondo local nativo. |
| `HeroSceneModelBindings.cs`, `HeroApprovedIdlePose.cs`, `HeroWeaponSocket.cs`, `HeroPreviewLoadout.cs` en Runtime | Cesión/restauración de modelos, poses y armas. |
| `HeroNaturalIdlePose.cs` en Runtime; `Assets/Editor/WorldHeroesCompactRevision.cs` | Corrección de brazos y muñecas sobre el rig original durante Idle; preparación idempotente y verificador protegido de la revisión compacta en copia aislada. |
| `HeroProgressStore.cs`, `HeroDevelopmentStore.cs`, `HeroDevelopmentService.cs`, `HeroEffectiveStats.cs`, `HeroResourcesBar.cs` en Runtime | Estado, operaciones, proyección de estadísticas y recursos. |
| `AeryxCompanionMotion.cs`, `AeryxObjectIdle.cs` en Runtime | Presentación del compañero original. |
| `Assets/Editor/WorldHeroesLargePanelsBuilder.cs`, `WorldHeroesLargePanelsValidation.cs`, `WorldHeroesGripPolish.cs`, `WorldHeroesTripoIntegration.cs` | Constructores y verificadores; inspeccionar condiciones y respaldos antes de ejecutarlos. |
| `Assets/WorldHeroesV2/Presentation/Kaeldor_Reactions.controller`, `Thorgrim_Reactions.controller`, `Thorgrim_Damage.anim` y `Assets/Editor/WorldHeroesDamageAnimationIntegration.cs` | Controladores derivados del original con reacción al daño y regreso al mismo reposo; adaptación Generic de Thorgrim sin modificar posiciones/escala de huesos ni FBX. Preparación protegida para copia aislada. Se restaura el controlador original al liberar el modelo de Village. |
| `Assets/RetargetingTrial/` | Ensayo separado, no rig de producción aprobado. |
| `Assets/WorldHeroesV2/Scenes/HeroesV2_Test.unity` | Escena histórica de pruebas, no escena principal. |
| `ArtSource/PanelesAprobados/Originales/`, `ArtSource/PanelesAprobados/` | Originales intactos, preparados e intermedios IA y salida 4K. |
| `Assets/WorldHeroesV2/Artwork/ApprovedPanels/` | PNG/sprites aprobados utilizados por Unity. |
| `Tools/ApprovedPanels/Prepare.ps1` | Preparación reproducible Upscayl/alfa/3840×2160; no reinstala herramientas. |
| `Validation/ApprovedPanels/`, `Validation/PanelFraming_20261026/` | Evidencia más reciente de paneles, manos y encuadres. |
| `Validation/TripoIntegration/`, `Validation/Aeryx/`, `Validation/RetargetingTrial/`, `Validation/HeroesConnected/` | Evidencia técnica histórica por ámbito. |
| `Backups/ApprovedPanels_20261026`, `HeroGripPolish_20261026`, `HeroDataConnection_20261026`, `PanelFraming_20261026`, `ProjectMemory_20261026` bajo Backups | Copias locales previas; pueden contener partida personal. No publicar en bloque. |

Informes previos conservados: `AERYX_INTEGRATION_STATUS.md`, `HEROES_PANEL_STATUS.md`, `HEROES_FUNCTIONAL_STATUS.md`, `HEROES_DEVELOPMENT_STATUS.md`, `HEROES_CONNECTED_STATUS.md`, `HEROES_STATS_UI_CORRECTIONS.md`, `HEROES_VILLAGE_COMPLETION.md`, `TRIPO_INTEGRATION_STATUS.md`, `WORLD_HEROES_PANELS_20261026.md` y `Validation/PanelFraming_20261026/Informe.md`. Son historia por fecha: algunas afirmaciones antiguas de modelos ausentes, seis ranuras, guiones o Volver principal han quedado sustituidas por el estado aquí descrito. No borrarlos ni aplicar automáticamente sus constructores como si fueran instrucciones actuales.

## 12. Última entrega, siguiente tarea y sincronización

**Última tarea COMPLETADA y COMPROBADA:** navegación exclusivamente con cuatro botones inferiores; superiores duplicados inactivos, HUD compartido arriba y arma original visible identificada en Equipo. 173 pruebas aisladas y clics nativos de las cuatro secciones en Play principal. Evidencia: `Validation/FooterNavigation_20261027`. No se modificaron poses en esta entrega; los ajustes artísticos de cuatro héroes siguen pendientes. Las siguientes entregas anteriores se conservan como historial.


**Última tarea de producto COMPLETADA y COMPROBADA en copia aislada:** panel compacto original con cuatro pestañas internas y un solo visor; ocho ranuras sin «Vacío», valores desconocidos en blanco, acciones contextuales y HUD compartido de nivel/vida/XP. Corrección real de brazos y muñecas para Thorgrim, Altherion, Lyriana y Shadows; Kaeldor conservado. Martillo y dagas por mangos, bastón más largo/fino sin deformar el FBX, rostro aprobado de Shadows visible y apoyo de Thorgrim comprobado durante animación. Renders en distintos ángulos y agarres cercanos, pruebas de UI/ratón/transacciones en `Validation/CompactRevision`. Copia segura inicial: `Backups/CompactRevision_20261026` (encargo iniciado el 26 y continuado el 27). Se trasladan siete assets derivados verificados y scripts al proyecto principal; no se reemplaza la escena guardada ni PNG/modelos originales. Las reacciones al daño anteriores se conservan. Aceptación artística final del usuario pendiente; no se ha avanzado al combate.

**Última tarea de mantenimiento COMPLETADA:** ambos documentos sincronizados y comprobados en GitHub main, sin publicar el proyecto completo; registro actualizado con los avances de animación. No se han importado paquetes de terceros.

**Siguiente tarea recomendada — PENDIENTE:** revisar poses y agarres de Thorgrim, Shadows, Altherion y Lyriana para aceptación artística, especialmente Thorgrim y su apoyo. La navegación inferior ya está comprobada en Play principal; no reconstruirla. Resolver cualquier defecto observado antes de ampliar animaciones de juego o avanzar al combate. Recuperar los datos reales faltantes de habilidades, equipo, evolución, mundos y atributos sin inventarlos.

**Git/GitHub — COMPROBADO (26/10/2026):** `origin` → `https://github.com/Nugenodget/world-heroes.git`, rama `main`. Sincronizados únicamente `AGENTS.md` y `WORLD_HEROES_ESTADO.md`, mediante avance normal sin force-push ni cambios del proyecto. El commit documental `31b7b35` se verificó con `git ls-remote` y la API de contenidos de GitHub: ambos blobs remotos coinciden con Git local. Revisión de contenido y patrones sensibles superada. Esta actualización registra esa comprobación. No afirmar que el juego completo esté respaldado en GitHub: sus nuevos assets/scripts siguen fuera del commit documental. Antes de sincronizar de nuevo, comprobar remoto, commits y archivos exactos para no sobrescribir trabajo ni publicar contenido ajeno al encargo.

No añadir en bloque `Backups`, `UserSettings`, logs, partidas reales, credenciales, claves/API, paquetes de terceros o cachés. El `.gitignore` actual es mínimo; preparar una política completa antes de un futuro `git add .`. No guardar secretos en este archivo. Las evidencias locales enlazadas pueden no estar aún en el remoto.

**Cómo consultar:** en una sesión con acceso a este repositorio, pedir «Lee AGENTS.md y WORLD_HEROES_ESTADO.md y resume lo comprobado, los bloqueos y el siguiente paso». En un chat sin acceso al repositorio, adjuntar o pegar la versión actual del archivo; no asumir acceso al disco ni actualización automática entre chats. La regla de AGENTS exige actualizar al finalizar el trabajo importante; no es un proceso en segundo plano que observa Unity o GitHub continuamente.

## Historial de decisiones importantes

| Fecha / fuente | Decisión o cambio conservado |
| --- | --- |
| 22/10/2026 — informes de integración | Aeryx original exclusivo de Kaeldor; store único y operaciones de progreso/inventario; presentación y pruebas separadas de combate real. |
| 23/10/2026 — RetargetingTrial | Ensayo Humanoid Kaeldor→Thorgrim válido técnicamente; aceptación artística pendiente y producción Generic conservada. |
| 24/10/2026 — Tripo/estadísticas | Prefabs y armas originales reutilizables; corrección de Thorgrim conservada; perfil provisional explícito para cuatro héroes; no inventar atributos adicionales. |
| 26/10/2026 — encargo de cuatro paneles | Diseños aprobados, Upscayl digital-art-4x, 4K/alfa, cuatro pantallas, Volver por pantalla, X principal, 25 habilidades con datos dinámicos; evolución separada de XP. |
| 26/10/2026 — recuperación y agarres | Shadows original recuperado y dos dagas; Thorgrim reutiliza prefab original por binding sin renderer; bastón al 72 %; contacto fino no declarado terminado. |
| 26/10/2026 — corrección del adjunto | Habilidades correcto ya coincidía por hash; no reprocesar ni usar el duplicado de Evolución. |
| 26/10/2026 — ajuste visual | Encuadres distintos por panel y fondo local de Unity; originales intactos; 141 comprobaciones aisladas. |
| 26/10/2026 — memoria permanente | Este archivo pasa a ser registro maestro; AGENTS exige leerlo y mantenerlo; alcance de siete mundos preservado aunque falten sus fichas. |
| 26/10/2026 — sincronización autorizada | Ambos documentos comprobados en GitHub main por su hash de blob; sin publicar el proyecto ni reescribir historial. |
| 26/10/2026 — daño de los guerreros | Reutilizado `hit_to_stomach` para Kaeldor y adaptado por rotaciones para Thorgrim, con controladores derivados y regreso a reposos aprobados. Corregido recorte del martillo en Equipo. 153 pruebas aisladas. La reserialización aclara el marcador `i` de XP sin cambiar los 19 valores. |
| 27/10/2026 — rediseño prioritario, sustituye navegación grande | El usuario exige panel compacto original con cuatro pestañas, un visor y datos/acciones contextuales. Quedan sustituidos los cuatro subpaneles grandes y sus encuadres independientes; recursos históricos conservados inactivos. Kaeldor se mantiene; prioridad real a brazos/apoyo de Thorgrim, bastón largo y fino, arco natural, Shadows con rostro y dagas por mangos. No avanzar a Match-3 hasta corregir panel y personajes. |

| 27/10/2026 — decisión definitiva de navegación | Las cuatro pantallas grandes quedan RECHAZADAS. Exclusivamente cuatro botones INFERIORES: Información, Equipo, Habilidades y Evolución; desactivar superiores duplicados. HUD compartido arriba, sin cubrir navegación. Armas originales visibles identificadas sin inventar inventario. Correcciones artísticas de cuatro héroes siguen pendientes; Kaeldor intacto. Esta decisión sustituye expresamente las aprobaciones históricas de ventanas grandes. |
