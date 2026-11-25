# CELIA — Manifiesto de recursos, imágenes y accesos

**Ruta canónica recomendada:** `docs/recursos/MANIFIESTO_RECURSOS_CELIA.md`  
**Versión:** 2.1.0  
**Fecha:** 2026-11-25  
**Estado:** Nueva documentación de CELIA y MATÍAS en GitHub; imágenes originales nuevas pendientes de carga binaria y QA. Los originales anteriores se consideran OBSOLETOS para nuevas publicaciones.

## 1. Propósito

Este documento es el **índice único** que indica a ChatGPT, Claude, Codex y otros agentes **qué recursos existen, dónde se encuentran, cuál está aprobado y qué uso se autoriza**.

**Regla:** no citar una imagen, ficha o audio como disponible solamente porque se mencionó en un chat. Debe existir el archivo, la ruta y una verificación de acceso. El nombre y ubicación final se completarán al cargar los materiales.

## 2. Ubicación de referencia del repositorio

- **Repositorio existente:** `jmmode/celia-ai`.
- **Visibilidad recomendada:** **privada**. **Estado observado 2026-11-24: PÚBLICO**; restringir si las fuentes visuales o documentos tienen derechos limitados.
- **URL GitHub verificada:** `https://github.com/jmmode/celia-ai` (**visibilidad observada: pública**).
- **Rama estable:** `main`.
- **Entrada humana:** `README.md`.
- **Entrada de agentes:** `CELIA_INSTRUCCIONES_PROYECTO.md`, `CLAUDE.md` y **este manifiesto**.
- **Autenticación:** GitHub connector / GitHub App / acceso autorizado de solo lectura. El acceso NO está configurado todavía.

**Importante:** no se requiere que el repositorio GitHub sea público. Para que Claude, ChatGPT o un agente puedan leerlo, deben contar con un conector o credenciales autorizadas por el propietario. No colocar secretos de acceso dentro de los archivos MD.

## 3. Árbol canónico de recursos

```text
celia-ai/
├── README.md
├── CLAUDE.md
├── CELIA_INSTRUCCIONES_PROYECTO.md
├── docs/
│   ├── identidad/
│   │   ├── FICHA_TECNICA_CELIA.md
│   │   ├── IDENTIDAD_VISUAL.md
│   │   └── IDENTIDAD_SONORA.md
│   ├── procedimientos/
│   │   └── FIRE_STICK_DOWNLOADER.md
│   ├── gobierno/
│   │   ├── DECISIONES_APROBADAS.md
│   │   └── POLITICA_CALIDAD.md
│   └── recursos/
│       └── MANIFIESTO_RECURSOS_CELIA.md
├── assets/
│   ├── identidad/       # fichas maestras visuales (PNG/JPG/WEBP/PDF autorizado)
│   ├── logos/           # logos maestros y derivados aprobados
│   ├── guias/           # guías gráficas, incluida Fire Stick
│   ├── capturas/        # pantallas reales Fire TV, Downloader, permisos, TiviPlay
│   └── audio/           # muestras autorizadas ligeras; no incluir secretos
├── producciones/
│   └── fire-stick-downloader/
│       ├── BRIEF.md
│       ├── GUION.md
│       ├── STORYBOARD.md
│       ├── QA.md
│       └── referencias.md
└── .gitignore
```

## 4. Registro de recursos pendiente de carga

| ID | Recurso | Ubicación destino en Git | Estado | Control previo a aprobación |
|---|---|---|---|---|
| CELIA-IMG-001 | Ficha maestra visual frontal de CELIA | `assets/identidad/celia-ficha-frontal.*` | PENDIENTE_CARGA | Verificar que es la ficha oficial |
| CELIA-IMG-002 | Ficha maestra visual complementaria de CELIA | `assets/identidad/celia-ficha-complementaria.*` | PENDIENTE_CARGA | Identidad facial/corporal consistente |
| CELIA-DOC-001 | Ficha técnica oficial (texto/PDF) | `assets/identidad/celia-ficha-tecnica.*` | PENDIENTE_CARGA | Extraer datos verificados a `docs/identidad/FICHA_TECNICA_CELIA.md` |
| CELIA-LOGO-001 | Logo principal TiviPlay Latino | `assets/logos/tiviplay-logo-principal.*` | PENDIENTE_CARGA | Fondo transparente/versión aprobada |
| CELIA-IMG-003 | Guía visual de instalación Fire Stick | `assets/guias/fire-stick-downloader-guia.*` | PENDIENTE_CARGA | Validar código y pasos |
| CELIA-IMG-004 | Guía de instalación Samsung (referencia de diseño, NO de flujo técnico) | `assets/guias/samsung-smarter-guia.*` | PENDIENTE_CARGA | Mantener separado de Fire Stick |
| CELIA-IMG-005 | Ícono oficial de Downloader | `assets/capturas/downloader-icono.*` | PENDIENTE_CARGA | Verificar integridad visual |
| CELIA-IMG-006 | Pantalla de inicio/búsqueda Fire TV | `assets/capturas/fire-tv-busqueda.*` | PENDIENTE_CARGA | Identificar versión Fire OS |
| CELIA-IMG-007 | Pantalla de Downloader con campo de código | `assets/capturas/downloader-codigo.*` | PENDIENTE_CARGA | Comprobar 2865004 |
| CELIA-IMG-008 | Opciones para desarrollador / aplicaciones desconocidas | `assets/capturas/fire-tv-permisos.*` | PENDIENTE_CARGA | Documentar modelo/versión |
| CELIA-IMG-009 | Pantalla de instalación y apertura de TiviPlay | `assets/capturas/tiviplay-instalar-abrir.*` | PENDIENTE_CARGA | Sin credenciales visibles |
| CELIA-IMG-010 | Pantalla de inicio de sesión de TiviPlay | `assets/capturas/tiviplay-acceso.*` | PENDIENTE_CARGA | Borrar usuarios/contraseñas reales |
| CELIA-AUDIO-001 | Referencia de voz oficial de CELIA | `docs/identidad/IDENTIDAD_SONORA.md` | REQUIERE_VALIDACION | Confirmar Agent ID/Voice ID con ElevenLabs |
| CELIA-VID-001 | MP4 final aprobado del tutorial | Almacenamiento de video gobernado (URL en `producciones/.../referencias.md`) | NO_PRODUCIDO | Control de calidad y aprobación |

> `*` significa que la extensión dependerá del formato real de los archivos que cargue el propietario. **No crear archivos vacíos como sustitutos de materiales faltantes.**

## 5. Ficha obligatoria por recurso

Para cada archivo incorporado, agregar un registro con estos campos:

```yaml
id: CELIA-IMG-XXX
nombre: nombre-real.ext
ruta_git: assets/carpeta/nombre-real.ext
sha256: PENDIENTE
origen: carga-del-propietario
fecha_ingreso: YYYY-MM-DD
version: '1.0'
estado: EN_REVISION # APROBADO | OBSOLETO
aprobado_por: PENDIENTE
uso_permitido: referencia-y-produccion-interna
licencia_o_autorizacion: PENDIENTE
contenido_sensible: false
notas: ''
```

La suma de `ruta_git` y `sha256` evita sustituir recursos visuales silenciosamente en nuevas generaciones.

## 6. Acceso público frente a privado

### Privado, recomendado para fuente maestra

`github.com/<organizacion-o-usuario>/celia-ai` **será accesible únicamente tras crear el repositorio y conceder permisos**. Esta cadena es un patrón, no una URL existente.

Los agentes autorizados deben acceder mediante GitHub/connector con permisos mínimos y leer archivos Markdown y medios permitidos. La colaboración sobre documentos debe quedar auditada mediante commits y PR.

### Público, únicamente si se decide publicar un paquete depurado

Propuesta opcional: un segundo repositorio público `celia-public-assets` o un sitio de documentación con **solo materiales explícitamente aprobados para difusión**: logo promocional, guía final pública, instrucciones genéricas para clientes. No publicar fichas maestras completas, claves, secretos, imágenes con permisos inciertos o información de clientes sin autorización.

### Alternativa de almacenamiento de archivos pesados

Audio de referencia y video final pueden guardarse en un Drive gobernado o almacenamiento de objetos con permisos controlados. En GitHub se documenta una **ruta/URI autorizada estable**, el propietario, versión y checksum; evitar enlaces efímeros o URLs con tokens.

## 7. Procedimiento de incorporación de los próximos adjuntos

1. Cargar las fichas, logos, guías y capturas en esta conversación.
2. Inspeccionar cada archivo realmente recibido; registrar extensión, resolución si aplica, y metadatos relevantes.
3. Clasificarlo según el inventario anterior; revisar duplicados y versiones.
4. Eliminar u ocultar información privada expuesta (usuarios, contraseñas, correos, enlaces internos sensibles).
5. Comprobar permisos de uso y marcar `EN_REVISION` antes de aprobación.
6. Renombrar sistemáticamente y ubicar en la ruta canónica.
7. Calcular SHA-256 y actualizar este manifiesto.
8. Crear commit / PR tras disponer del repositorio, verificar que los enlaces internos funcionan.
9. Cambiar a `APROBADO` solo después de revisión del responsable.

## 8. Contrato de lectura de cualquier agente

**Consulta recomendada:**

> Lee `CELIA_INSTRUCCIONES_PROYECTO.md` y `docs/recursos/MANIFIESTO_RECURSOS_CELIA.md` del repositorio `celia-ai` al que tienes acceso. Para cada recurso, localiza la ruta canónica, revisa el estado y usa exclusivamente archivos `APROBADO`. Si la ficha, el logo, la imagen o el audio no están disponibles, señala la dependencia y no inventes sustitutos. Indica las rutas y versiones que realmente consultaste.

## 9. Estado de construcción

**Completado:** definición de rutas, roles, estructura de acceso y registro inicial basado en el trabajo ya aprobado.  
**Pendiente:** subida de imágenes originales a GitHub, verificación de voz oficial, validación de activos, habilitación de permisos de lectura para Claude y demás agentes.

## 10. Migración de identidad gráfica — 2026-11-24

- **CELIA-V2-DOC**: `docs/identidad/FICHA_TECNICA_CELIA.md` — DOCUMENTADO.
- **MATIAS-V1-DOC**: `docs/identidad/FICHA_TECNICA_MATIAS.md` — DOCUMENTADO.
- **BRAND-V2-DOC**: `docs/identidad/IDENTIDAD_VISUAL.md` — DOCUMENTADO.
- **CELIA-V2-IMG**: nueva ficha `ficha_maestra_de_celia_tiviplay_latino.png` (archivo del chat) — PENDIENTE_CARGA_GITHUB_DRIVE y revisión de erratas en textos pequeños.
- **MATIAS-V1-IMG**: `ficha_maestra_de_mateo_tiviplay_latino.png` (archivo del chat) — PENDIENTE_CARGA_GITHUB_DRIVE y QA.
- **CELIA-LEGACY-IMG-001/002**: fichas del avatar previo — **OBSOLETO_PARA_PRODUCCION**, pendiente de eliminación después de verificar sustitutos y dependencias. No borrar automáticamente.
- **CELIA-VOICE**: agente `agent_1501m7x7hjy8escav3sta1gakbmq`, Voice ID `EYBbN7OENxAX5QX56IiW` — CONSERVAR.
- **MATIAS-VOICE**: Yorman Zapata - Podcast, Ads; `VVBVYefvg7r5n2yHrobQ` — VALIDADO. Contrato: `docs/identidad/TIVIPLAY_IDENTIDAD_VOCAL_MATIAS_V1_2026-11-25.md`.

**Regla de migración:** actualizar los agentes lectores para que consulten los documentos nuevos; prohibir la reutilización de fichas anteriores incluso mientras sigan archivadas. No inventar hashes ni afirmar que las nuevas imágenes están cargadas antes de verificar los binarios.
