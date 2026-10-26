# WORLD HEROES — registro maestro permanente

Última actualización: **26/10/2026, Europe/Madrid**. Fuente de estado vigente del repositorio; leer junto con `AGENTS.md` antes de trabajar. Este archivo registra decisiones, implementación y evidencia; no sustituye la inspección del proyecto ni convierte una intención en una función terminada.

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
5. Conservar los cuatro diseños aprobados, dragón Aeryx, marcos y adornos. Originales intactos, mejora IA real con Upscayl `digital-art-4x`, salida 3840 × 2160, proporciones conservadas y alfa real. No inventar transparencias ni eliminar los interiores azules. No instalar herramientas adicionales sin explicarlas previamente.
6. Información y Equipo conservan su alfa. Habilidades y Evolución retiran únicamente el negro previsto como ventana transparente. Evitar halos; comprobar visualmente. El adorno inferior no debe tapar Vida/XP. Los datos variables pertenecen a Unity/TMP, nunca a nuevos textos pintados en PNG.
7. Cuatro pantallas grandes independientes: Información, Equipo, Habilidades, Evolución. Abrir una oculta el principal; cada una tiene flecha dorada Volver reutilizable y en la misma posición. Volver conserva la selección. **Solo la X principal cierra Héroes y vuelve a Village.** Apariencia existente se conserva.
8. Interfaz 16:9, incluida 1080p y 4K; sin deformar, con efectos suaves azules. Mismo modelo real, giro de ratón y animaciones existentes.
9. Presentación vigente: Información grande desde muslos; Equipo cuerpo entero; Habilidades sin 3D sobre iconos/texto; Evolución grande aproximadamente desde rodillas. Fondo azul oscuro local creado en Unity, sin modificar PNG ni adornos. Cámara/encuadre propios por panel; restaurar el principal al volver.
10. Estadísticas, inventario y recursos reales y sincronizados. Cero confirmado se muestra como `0`; dato ausente se identifica, no se transforma indiscriminadamente en cero. No inventar objetos, habilidades, costes, evoluciones, modelos ni recursos.
11. Vida inicial llena y XP vacía al nivel 1. Daño reduce vida; XP aumenta y sube niveles automáticamente, gratis y sin curación implícita. Evolución especial es un sistema diferente que consume recursos ganados jugando cuando sus reglas existan.
12. Seis estadísticas requeridas: Ataque, Defensa, Velocidad, Crítico, Resistencia y Precisión; además vida, XP y maná/recurso de clase cuando exista. Respetar los hitos de vida ya definidos.
13. Habilidades: cinco por héroe, selección de icono central y **nombre dinámico inmediatamente debajo**, descripción, nivel 1–20, daño/efecto, recarga, costes oro/cristales y Mejora validada. Equipo: ranuras, Equipar/Mejorar/Quitar reales. Evolución: nombre/rango, niveles actual/siguiente, seis estadísticas actuales/futuras y requisitos reales.
14. Armas originales en sus manos, acompañando la animación; ajustar individualmente agarre y dedos. Kaeldor es referencia inicial, sin imponer espada a arco o bastón. Pose T solo como referencia de rig. Respetar correcciones aprobadas de Thorgrim; reducir bastón de Altherion; Shadows debe usar su 3D original y dos dagas; Lyriana conserva arco y diseño.
15. Orden aprobado del encargo amplio: paneles → Kaeldor/Thorgrim → Altherion/Shadows/Lyriana → contadores. No repetir tareas ya resueltas. Actualizar este registro después de entregas importantes y dar informe breve en español.

## 3. Héroes, Aeryx, enemigos y siete mundos

| Personaje | Rol aprobado | Modelo/arma vigente | Estado real |
| --- | --- | --- | --- |
| Kaeldor | Guerrero | Original `Kaeldor/kaeldor.fbx`; espada `Espada_Kaeldor_1`, derecha | COMPROBADO: 3D, reposo, giro y anclaje; contacto fino de dedos PENDIENTE. |
| Thorgrim | Enano guerrero | Original `thorgrim/thorgrim.fbx` mediante `Thorgrim_Reusable`; martillo izquierdo | COMPROBADO: modelo, pose aprobada y anclaje; acabado fino PENDIENTE. |
| Altherion | Mago | Original `Altherion_1/Altherion_1.fbx`; bastón derecho | COMPROBADO: reposo, anclaje y reducción uniforme del bastón al 72 % de su escala anterior; acabado fino PENDIENTE. |
| Shadows | Asesino | Original `fantasy_armored_warrior_3d_model/...fbx`, con rostro; dos dagas | COMPROBADO: original recuperado con GUID/materiales, visor 3D y dos anclajes; acabado fino PENDIENTE. |
| Lyriana | Arquera | Original `Lyriana/Lyriana.fbx`; arco izquierdo | COMPROBADO: 3D, reposo y anclaje original; acabado fino PENDIENTE. |
| Aeryx | Compañero de Kaeldor | `AeryxRiggedOriginal` / `AeryxOriginalCompanion.prefab` | COMPROBADO históricamente: solo con Kaeldor, cuatro apoyos, respiración/cabeza y giro independiente. En subpaneles se oculta su 3D porque el PNG ya incluye Aeryx. |

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

## 4. Cuatro paneles: estado real

**COMPLETADO y COMPROBADO en copia aislada:** cuatro PNG mejorados mediante IA, alfa revisado, controles nativos, navegación, selección conservada y cierre principal. Los cuatro originales coinciden con sus hashes. Habilidades correcto: `file_000000004cf08246ac3f0497d6404d2f.png`; la repetición adjunta de Evolución no se utilizó como Habilidades.

| Panel | Implementación y comprobación | Pendientes/dependencias |
| --- | --- | --- |
| Información | Modelo real giratorio, nombre/clase/nivel, seis campos, vida/XP dinámicas; encuadre desde muslos y fondo local. | Estadísticas adicionales y balance definitivo de cuatro héroes. |
| Equipo | Cuerpo entero, ocho ranuras, inventario compatible, equipar/quitar y estadísticas efectivas del mismo store. | Catálogo de producción y sistema real de mejora de objetos; acciones sin datos desactivadas. |
| Habilidades | Cinco selecciones, icono central, nombre TMP justo debajo, descripción/nivel/efecto/recarga/costes; confirmación y tope 20 probados con datos TEST. Sin 3D superpuesto. | Nombres, efectos, costes, desbloqueos y recargas reales de las 25 habilidades. |
| Evolución | Modelo desde rodillas, nombre/rango, comparación y requisitos dinámicos preparados, Vida/XP sincronizadas. | `IHeroEvolutionSource` real y reglas/modelos aprobados; Evolucionar desactivado mientras falten. |

Las pruebas con datos TEST verifican operaciones, no conceden equipo o recursos al jugador ni demuestran contenido definitivo. El castillo visible proviene del gráfico aprobado existente; Village 3D sigue siendo geometría de prototipo. El fondo local nuevo despeja exclusivamente el retrato; no reemplaza la aldea.

**Evidencia:** `Validation/ApprovedPanels/ImagesManifest.json`, `ImageChecks.txt`, `PlayChecksFinal.txt` (79 comprobaciones), `FinalScreens`, `FinalHands`; después `Validation/PanelFraming_20261026/PlayChecks.txt` (**141 comprobaciones**, cinco héroes × tres encuadres, navegación, restauración principal y regresión), `Screens`, `Unity.log`, `Preservation.json`. Capturas de cuatro paneles en 1080p y 4K; quince encuadres individuales en 1080p. Compilación y Play comprobados en copia aislada `Temp/ApprovedPanelsValidation`; no se atribuye a esta pasada una nueva aceptación manual del usuario en el editor principal.

## 5. Modelos, armas, rigging y animaciones

**COMPROBADO:** se conservan FBX, materiales y texturas originales. Los rigs de producción son Generic, sin certificar Humanoid de producción. Anclajes `Grip`/`HeroWeaponSocket` siguen la palma; poses locales de cierre sobreviven al reposo. Esto no certifica contacto artístico perfecto de cada dedo con cada empuñadura.

Reposos usados: Kaeldor `wait (1)`/estado `wait`; Thorgrim clip `idle.001`/estado `idle_001`; otros tres `Altherion_PanelIdle`, `Lyriana_PanelIdle`, `Shadows_PanelIdle`, adaptados sobre sus propios rigs. Se conservan controladores y correcciones de brazos aprobadas, con aplicación después del Animator cuando corresponde. No se ha forzado una animación de espada a arco/bastón.

Thorgrim: el objeto de escena `reposo` no tenía renderizadores y su binding estaba vacío. Se reutiliza el prefab existente del FBX original con `HeroApprovedIdlePose`; se conservan los objetos vacíos y los valores aprobados. Shadows: el original faltaba en disco y se recuperó mediante copia desde la Papelera; no se generó un sustituto. El montaje usa dos instancias del recurso de daga original, una por mano.

**COMPROBADO solo como ensayo aislado:** retargeting Humanoid Kaeldor → Thorgrim para reposo y caminar, Avatars válidos y reproducción real. `Assets/RetargetingTrial` y `Validation/RetargetingTrial` conservan pruebas. Apoyo, deslizamiento y diferencias de postura no tienen aprobación artística final; no migrar producción por el mero hecho de que `Avatar.isValid` sea verdadero.

**PENDIENTE:** ajustar contacto artístico de dedos/pulgar y armas, revisar muñecas y postura desde varios ángulos, revisar animaciones completas de juego. La orientación automática uniforme de armas se probó aisladamente y se descartó porque empeoraba el arco; no aplicarla al proyecto principal.

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
| Reposo | COMPROBADO en presentación de los cinco héroes; Aeryx procedimental. Reposo de combate por clase PENDIENTE. |
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

**PENDIENTE:** tablero, turnos, reglas de combinaciones, objetivos, daño, recarga, selección de enemigos, premios y resultado. No se ha encontrado un motor Match-3 funcional en los scripts revisados. La existencia de `World1_Level1.unity` no cambia esta conclusión.

**BLOQUEADO para conexión definitiva:** faltan reglas de combate y contenido confirmado. Una vez definidos, enlazar reposo/movimiento/ataque/habilidad/defensa/daño/victoria/derrota con eventos reales del combate, resolver los efectos una sola vez y enviar resultados al almacén compartido. No mantener estadísticas, carteras o XP paralelas, ni usar animaciones como prueba de combate terminado.

## 9. Recursos, estadísticas, XP, evolución, inventario y habilidades

- **COMPROBADO — fuente única:** `HeroProgressStore.Shared`, persistencia `Application.persistentDataPath/world-heroes-v2.json`, lectura efectiva de base + nivel + mejoras configuradas + equipo. Eventos comunes actualizan menú y subpaneles. No incorporar el guardado real a Git.
- **COMPROBADO — transacciones:** pruebas aisladas de equipar/quitar, mejoras con confirmación, costes exactos, rechazo de doble operación, máximos y persistencia. Las pruebas históricas más amplias están en `Validation/HeroesConnected`; no confundir sus fixtures con datos de producción.
- **BLOQUEADO — recursos jugables:** madera, oro, metal y cristales existen como contrato, pero la partida real tiene `resourcesKnown = false`. Se muestra `Sin conectar`. No inicializar saldos de ejemplo. Cero confirmado se muestra como `0` y cambia por evento real.
- **COMPROBADO — Kaeldor:** nivel inicial 1; vida base 100, ataque 25, defensa 20, velocidad 15, poder 30. Hitos de vida máxima base 1→100, 10→110, 20→120. Tabla existente de XP 100, 200, …, 1900 para niveles 1→20; no extrapolar después del límite.
- **COMPROBADO — otros cuatro:** perfil compartido `ProvisionalInitialStats.asset` inicializa registros independientes con el baseline existente y aviso de provisionalidad. No es balance definitivo de sus clases ni sobrescribe el progreso guardado. **PENDIENTE** aprobar atributos individuales.
- **PENDIENTE — adicionales:** crítico, resistencia, precisión y maná/recurso de clase carecen de valores aprobados; `Sin definir`. No transformar campos internos cero en cifras reales.
- **COMPROBADO — vida/XP:** mismo estado en todas las pantallas, daño/curación explícitos, XP gratuita automática, vida actual conservada al subir nivel y hitos comprobados. El combate todavía no concede premios reales.
- **COMPLETADO como operaciones, BLOQUEADO por contenido — inventario:** equipamiento real por ID, compatibilidad, propiedad y estadísticas efectivas sin acumular bonos al releer. Ocho ranuras visuales; los seis IDs originales se preservan y Gloves/OffHand se añaden al final. No hay catálogo jugable aprobado ni objetos concedidos al jugador. Mejorar equipo requiere proveedor real.
- **COMPLETADO como estructura, BLOQUEADO por contenido — habilidades:** 25 IDs estables, cinco por héroe; selección/nombre/icono, rangos hasta 20, requisitos y confirmación. Assets con `skillConfigured = false`, sin efectos/costes finales. No activar con datos ficticios.
- **PENDIENTE — evolución especial:** `IHeroEvolutionSource` y comparación preparados; no hay proveedor definitivo, rangos, costes o modelos aprobados. No confundir con las mejoras individuales de atributos heredadas (`attributeUpgrades`) ni con nivel gratuito por XP. Nunca inventar una evolución o gastar recursos sin regla real.

## 10. Errores conocidos, pendientes y prioridades

| Prioridad | Tarea o incidencia | Estado y dependencia |
| --- | --- | --- |
| 1 | Aceptación visual de los encuadres nuevos en el editor principal y revisión fina de manos/armas en cinco héroes | PENDIENTE. Las pruebas aisladas y capturas no equivalen a aprobación artística. |
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

**Última tarea de producto COMPLETADA y COMPROBADA:** daño real conectado a las reacciones de Kaeldor y Thorgrim, con regreso a sus reposos y restauración del controlador original al liberar el modelo. Thorgrim reutiliza los deltas del clip de Kaeldor sobre 65 huesos coincidentes, partiendo de su pose aprobada; no se transfieren posiciones ni escalas. Controladores derivados, clip adaptado y definiciones verificados trasladados al proyecto principal, sin tocar FBX ni controladores fuente. Equipo ajusta la cámara incluyendo las armas montadas durante la animación; se corrigió el recorte del martillo detectado en la prueba visual. **153 comprobaciones aisladas superadas**, con movimiento real de columna, giro conservado, daño cero rechazado, vuelta a reposo, restauración de Village y regresión de los cinco héroes/paneles. Evidencia en `Validation/DamageAnimation_20261026/`; copia previa en `Backups/AnimationDamage_20261026`. Los encuadres y el fondo local anteriores siguen conservados. La reserialización confirmó que el sufijo `i` de XP lo conserva Unity: no se han cambiado requisitos ni hitos. La revisión artística fina de manos y nuevas animaciones sigue pendiente, y esto no constituye un motor de combate Match-3.

**Última tarea de mantenimiento COMPLETADA:** ambos documentos sincronizados y comprobados en GitHub main, sin publicar el proyecto completo; registro actualizado con los avances de animación. No se han importado paquetes de terceros.

**Siguiente tarea recomendada — PENDIENTE:** verificar visualmente los cinco héroes con los nuevos encuadres en Play de Village y ajustar contacto artístico de las armas sin alterar originales. Después, auditar los paquetes descargados y probar animaciones compatibles de Kaeldor/Thorgrim en aislamiento antes de conectarlas al juego. Recuperar en paralelo la documentación faltante de mundos y contenido; no inventarla.

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
