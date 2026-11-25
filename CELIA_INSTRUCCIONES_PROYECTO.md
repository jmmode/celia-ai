# CELIA — Instrucciones maestras del proyecto

**Documento:** `CELIA_INSTRUCCIONES_PROYECTO.md`  
**Versión:** 2.1.0  
**Fecha de consolidación:** 2026-11-25  
**Estado:** Identidad gráfica original CELIA/MATÍAS documentada; nueva ficha binaria pendiente de carga y QA.  
**Responsable de aprobación:** Dirección del proyecto CELIA / TiviPlay Latino.

## 1. Propósito

CELIA es la identidad de asistente virtual y presentadora audiovisual de TiviPlay Latino. Su nombre y voz se conservan; la imagen previa queda obsoleta y se sustituye por una identidad gráfica original. MATÍAS es su contraparte masculina visual para comunicación (voz oficial documentada; sin agente conversacional confirmado). Este proyecto organiza la documentación de su identidad, su voz, los procedimientos de servicio y los materiales de producción para que ChatGPT, Claude, Codex y otros agentes trabajen sobre **fuentes versionadas**, sin depender de conversaciones.

**Objetivo operativo:** producir y mantener contenidos de atención al cliente, tutoriales, guiones, audiovisuales y flujos de soporte coherentes con la marca y técnicamente verificables.

## 2. Fuentes de verdad y precedencia

Orden de autoridad para cualquier agente:

1. `docs/identidad/FICHA_TECNICA_CELIA.md` **validada**, junto con recursos maestros oficiales referenciados en el inventario.
2. `docs/gobierno/DECISIONES_APROBADAS.md` y las políticas de calidad vigentes.
3. Procedimientos técnicos aprobados en `docs/procedimientos/`.
4. Guiones, storyboards y briefs con estado `APROBADO` en `producciones/`.
5. Este documento y el `README.md` del repositorio.
6. Conversaciones y borradores: contexto de trabajo, **no fuente normativa**.

Si hay contradicción, **no inventar una conciliación**: registrar discrepancia y solicitar decisión. No convertir información pendiente en verificada.

## 3. Función de cada plataforma

- **ChatGPT, proyecto CELIA:** análisis, trabajo colaborativo, decisiones y elaboración de documentos.
- **GitHub, repositorio `jmmode/celia-ai` (existente):** fuente versionada principal de documentación, referencias y decisiones aprobadas.
- **Claude / Codex / otros agentes:** consumidores o colaboradores del repositorio, únicamente con permisos explícitos.
- **ElevenLabs:** plataforma de voz oficial; sus identificadores son referencias, no credenciales.
- **Almacenamiento de activos:** archivos pequeños versionados en Git; videos/audio pesados en almacenamiento gobernado, Git LFS o repositorio de medios según decisión técnica.

**Importante:** mover el chat al proyecto no sincroniza su contenido con GitHub. El repositorio tampoco es accesible para otros agentes hasta conceder acceso o entregar un archivo explícitamente.

## 4. Normas obligatorias para agentes

1. Leer `README.md`, `CLAUDE.md` (si es Claude) y este archivo al iniciar.
2. Consultar `docs/recursos/MANIFIESTO_RECURSOS_CELIA.md` para localizar logos, fichas, capturas y guías.
3. Leer la ficha oficial y las decisiones antes de representar o narrar a CELIA.
4. Mantener consistencia facial, corporal, de vestuario y de marca según material **aprobado**, sin fabricar variantes.
5. No cambiar la voz oficial por una voz genérica. Si falta acceso o confirmación de voz, registrar bloqueo.
6. No inventar enlaces, contraseñas, códigos, capturas de aplicaciones, permisos ni resultados de generación.
7. No afirmar que se produjo, publicó o validó un video sin archivo generado y comprobación real.
8. Registrar toda modificación sustancial mediante cambios versionados, responsable, fecha y estado.
9. No incluir credenciales de clientes, tokens, API keys, archivos confidenciales o información personal en el repositorio.
10. Distinguir claramente `BORRADOR`, `EN_REVISION`, `APROBADO` y `OBSOLETO`.

## 5. Identidad audiovisual CELIA

- **Rol:** presentadora y asistente virtual oficial de TiviPlay Latino.
- **Apariencia:** según `docs/identidad/FICHA_TECNICA_CELIA.md` e `IDENTIDAD_VISUAL.md` versión 2.0.0. La ficha histórica queda OBSOLETA para producción; la nueva imagen maestra requiere carga y revisión del binario.
- **Voz:** definida por el proyecto existente de ElevenLabs. En el historial del proyecto se ha usado el agente `CELIA | TiviPlay Latino | Prototipo`, Agent ID `agent_1501m7x7hjy8escav3sta1gakbmq`, voz referenciada como **Kate 1 — Warm, Close and Natural**, Voice ID `EYBbN7OENxAX5QX56IiW`. **Estos datos provienen de decisiones previas; deben confirmarse en ElevenLabs antes de generar audio definitivo.**
- **Advertencia:** una búsqueda por el nombre “Celia” mostró una voz pública francesa con otro identificador; **no corresponde a una verificación de la voz oficial** y no se debe sustituir la referencia previa por esa coincidencia nominal.
- **Estilo narrativo:** español latinoamericano, profesional, claro, cercano y orientado a servicio.

## 5.1 Identidad audiovisual Matías

- Ficha: `docs/identidad/FICHA_TECNICA_MATIAS.md`.
- Voz oficial: Yorman Zapata - Podcast, Ads; Voice ID `VVBVYefvg7r5n2yHrobQ`.
- Contrato: `docs/identidad/TIVIPLAY_IDENTIDAD_VOCAL_MATIAS_V1_2026-11-25.md`.

## 6. Proyecto activo: instalación de TiviPlay en Amazon Fire Stick

**Objetivo:** video tutorial cinematográfico vertical con CELIA como protagonista para publicación en estados de WhatsApp.

**Dirección visual:** sala residencial moderna; CELIA con control remoto Fire Stick; alternar planos cinematográficos con interfaces reales y legibles proporcionadas por la marca. No confundir este flujo con Samsung, LG, Google TV o IPTV Smarters.

**Procedimiento aprobado:**

1. Pulsar **Home** en el Fire Stick.
2. Seleccionar lupa/búsqueda, buscar **Downloader**, instalarlo y abrirlo.
3. Si la instalación requiere permiso: `Configuración > Mi Fire TV > Opciones para desarrollador > Instalar aplicaciones desconocidas > Downloader > Activado`.
4. Si las opciones de desarrollador no son visibles: `Mi Fire TV > Acerca de > nombre del dispositivo`, presionar aproximadamente siete veces el botón de selección central y regresar al menú de desarrollador.
5. En Downloader, introducir el código **2865004**, pronunciarlo **dos, ocho, seis, cinco, cero, cero, cuatro**, y seleccionar **Go**.
6. Descargar el APK desde el destino esperado y seleccionar **Instalar** y luego **Abrir**.
7. Introducir los datos de acceso que suministre el asesor; **nunca publicar credenciales reales**.

**Nota de seguridad:** habilitar únicamente el permiso necesario para Downloader, cuando aparezca; **no activar la depuración ADB de forma predeterminada**. Verificar el destino del código y la procedencia autorizada del APK antes de difundir instrucciones, y revisar la ruta exacta en los modelos/versiones relevantes de Fire OS.

**Duración aprobada como objetivo de producción:** flexible, aproximadamente **35–45 segundos**, subordinada a la locución real y legibilidad. **Formato:** 9:16, objetivo 1080×1920, MP4 H.264. Comprobar requisitos vigentes de WhatsApp antes de publicar.

**Secuencia audiovisual:** introducción de CELIA; Home/búsqueda; permisos condicionales; apertura de Downloader/código; descarga/instalación; credenciales; cierre/soporte. Música discreta, subtítulos legibles y lip-sync con voz oficial.

## 7. Controles mínimos de calidad y aprobación

- [ ] Identidad facial/vestuario de CELIA conforme a las fichas aprobadas.
- [ ] Voz oficial verificada y utilizada (sin sustitución no aprobada).
- [ ] Diálogo y labios sincronizados.
- [ ] Fire Stick y Downloader representados sin interfaces de otras plataformas.
- [ ] Código `2865004` mostrado íntegro y narrado dígito a dígito.
- [ ] Orígenes desconocidos incluidos solo cuando el dispositivo lo exija; sin ADB innecesaria.
- [ ] Capturas oficiales, sin distorsiones ni inventos de UI.
- [ ] Datos de acceso ficticios/vacíos; no exponer datos de clientes.
- [ ] Audio, ortografía, encuadre y legibilidad revisados en pantalla móvil.
- [ ] Archivo final reproducible, metadatos de entrega y responsable de aprobación registrados.

## 8. Propuesta de estructura del repositorio

```text
celia-ai/
├── README.md
├── CLAUDE.md
├── CELIA_INSTRUCCIONES_PROYECTO.md
├── docs/
│   ├── identidad/
│   │   └── FICHA_TECNICA_CELIA.md
│   ├── gobierno/
│   │   ├── DECISIONES_APROBADAS.md
│   │   └── POLITICA_CALIDAD.md
│   ├── procedimientos/
│   │   └── FIRE_STICK_DOWNLOADER.md
│   └── recursos/
│       └── MANIFIESTO_RECURSOS_CELIA.md
├── assets/
│   ├── identidad/
│   ├── logos/
│   ├── guias/
│   └── capturas/
├── producciones/
│   └── fire-stick-downloader/
│       ├── BRIEF.md
│       ├── GUION.md
│       ├── STORYBOARD.md
│       └── QA.md
└── .gitignore
```

## 9. Política de publicación y acceso

**Opción recomendada:** repositorio **privado** con acceso de lectura para agentes y colaboradores autorizados. El repositorio puede tener rutas estructuradas y estables **sin hacerse público**.

- **Compartible a agentes autorizados:** instrucciones, fichas depuradas, guiones, guías, logos y capturas libres de secretos.
- **Solo acceso restringido:** materiales fuente con derechos de uso limitados, decisiones internas sensibles y originales sin depurar.
- **Nunca Git:** claves API, tokens, contraseñas de clientes, datos personales innecesarios, archivos `.env`, secretos de conectores.
- **Solo si se aprueba un repositorio público:** publicar una selección de documentos y activos revisados, separada del repositorio privado. No asumir que “público” es obligatorio para que Claude acceda.

## 10. Flujo de cambios

`PROPUESTA → REVISION_TECNICA → APROBACION_DIRECCION → VERSIONADO → USO_EN_PRODUCCION → AUDITORIA`

Todo agente debe indicar qué documentos utilizó (ruta y versión/commit cuando sea posible), qué cambió, qué quedó bloqueado y cuál es el entregable verificable.

## 11. Pendientes documentales

- [x] Documentar identidad visual original de CELIA y MATÍAS; [ ] adjuntar imágenes maestras nuevas y validar su QA.
- [ ] Adjuntar logos originales y verificar versiones aprobadas.
- [ ] Adjuntar imágenes guía y capturas de Fire Stick/Downloader.
- [ ] Confirmar en ElevenLabs Agent ID, Voice ID, acceso y licencia de uso de voz.
- [ ] Comprobar destino real del código `2865004` y fuente del archivo de instalación.
- [ ] Definir teléfono/contacto corporativo oficial en el cierre audiovisual.
- [ ] Formalizar guion, storyboard y política de aprobación del MP4.
- [ ] Crear repositorio y configurar accesos de lectura de Claude y demás agentes.

## 12. Instrucción estándar reutilizable

> Lee `README.md`, `CELIA_INSTRUCCIONES_PROYECTO.md` y `docs/recursos/MANIFIESTO_RECURSOS_CELIA.md` en la versión vigente del repositorio. Identifica los documentos aprobados aplicables, realiza la tarea sin sustituir recursos oficiales y reporta cualquier brecha documental. Cita rutas y versiones de los archivos consultados. No inventes hechos ni declares entregables no producidos.