# TiviPlay Latino — Identidad vocal de Matías

**Versión:** 1.0 · **Fecha:** 2026-11-25  
**Responsable:** JUMOCOL · **Área primaria:** 03 Comercial y Ventas · **Dependencia:** 04 Plataforma y Equipo

## 1. Decisión vigente

La voz oficial de Matías es **Yorman Zapata - Podcast, Ads**, de ElevenLabs. Seleccionada expresamente por dirección y verificada mediante consulta a la biblioteca de ElevenLabs el 25 de noviembre de 2026.

| Campo | Valor | Estado |
|---|---|---|
| Personaje | Matías (no Mateo) | VALIDADO |
| Proveedor | ElevenLabs | VALIDADO |
| Voz | Yorman Zapata - Podcast, Ads | VALIDADO |
| Voice ID | `VVBVYefvg7r5n2yHrobQ` | VALIDADO |
| Categoría | Voz profesional de biblioteca | VALIDADO |
| Idioma / acento | Español / colombiano | VALIDADO |
| Uso | Locución audiovisual, tutoriales y publicidad | Aprobado |
| Plan | Starter | Activación reportada por dirección |

## 2. Contrato técnico propuesto

Parámetros base recomendados; no constituyen evidencia de la configuración efectiva de una generación anterior. Para la API se usa `es` como código de idioma; `es-CO` describe la identidad regional.

```json
{
  "character": "MATIAS",
  "brand": "TiviPlay Latino",
  "version": "1.0",
  "voice_provider": "ElevenLabs",
  "voice_name": "Yorman Zapata - Podcast, Ads",
  "voice_id": "VVBVYefvg7r5n2yHrobQ",
  "model_id": "eleven_multilingual_v2",
  "locale": "es-CO",
  "language_code": "es",
  "voice_settings": {
    "speed": 1.0,
    "stability": 0.5,
    "similarity_boost": 0.75,
    "style": 0.0,
    "use_speaker_boost": true
  }
}
```

## 3. Primera producción — Tutorial de soporte

**Libreto aprobado:**

> ¡Hola! Soy Matías.
>
> Si la novedad continúa, estamos listos para ayudarte.
>
> Envíanos tu nombre, una foto o video de la novedad, indícanos en qué dispositivo ocurre y confírmanos si realizaste los dos pasos anteriores.
>
> En TiviPlay Latino, estamos para acompañarte.

Activo recibido: `ElevenLabs_2026-11-25T07_10_17_Yorman Zapata - Podcast, Ads_pvc_s50_m2.mp3`. Nombre operativo sugerido: `TIVIPLAY_MATIAS_TUTORIAL_SOPORTE_V01.mp3`. El archivo fue aportado por dirección; su contenido y configuración completa de síntesis no se han auditado en esta actualización.

## 4. Control de versiones y costos

- Marcus – Educational Narrative: selección anterior sustituida; no utilizar para Matías.
- `MATÍAS_TIVIPLAY_V1` (ID `n0sYLpoxdQ6oqO73TRut`): voz de diseño inicial guardada, posteriormente descartada para el personaje. No eliminada.
- Reutilizar el audio existente si supera el control de calidad. No regenerar muestras sin necesidad.
- Mantener el Voice ID como referencia en futuras integraciones; no sustituir automáticamente la voz si deja de estar disponible.
- Comprobar disponibilidad y condiciones comerciales de la voz antes de nuevos usos. La integración conversacional requiere validación propia.
- No almacenar claves API ni credenciales en este documento.

## 5. Checkpoint

**VALIDADO:** identidad vocal de Matías y coincidencia del Voice ID en ElevenLabs.  
**PARCIAL:** configuración técnica de síntesis propuesta; validación auditiva y montaje pendientes.  
**NEXT ACTION:** incorporar este delta al contrato maestro de identidad de TiviPlay en el repositorio vigente, verificar la identidad vocal de Celia por separado y finalizar el tutorial reutilizando el audio disponible.

No se han realizado cambios en GitHub, ElevenLabs ni Google Drive durante la elaboración de este documento. No se han generado audios adicionales.
