# Roadmap

## Fase 1 — Identidad (rebrand)

- [x] Definir nombre de la app → **Mazarin**
- [x] Cambiar package ID → `dev.qwertylab.mazarin`
- [ ] Nuevo icono y logo
- [ ] Actualizar splash screen con nuevo branding
- [x] Actualizar pantalla About (links, créditos, descripción)
- [x] Reemplazar/eliminar API key de Google Books hardcodeada
- [x] Cambiar `applicationId`, `versionName`, `versionCode`

## Fase 2 — Limpieza de código

- [ ] Migrar todo de Material 2 a Material 3 (eliminar dependencia `compose-material`)
- [x] Limpiar warnings de deprecación en `gradle.properties`
- [x] Verificar `.gitignore` (local.properties, keys, builds)
- [ ] Eliminar código muerto o comentado
- [ ] Revisar y limpiar strings hardcodeados (preparar para i18n)

## Fase 3 — Mejoras del lector

- [ ] Temas de lectura (claro, sepia, oscuro, AMOLED negro)
- [ ] Sistema de bookmarks/marcadores con persistencia en Room
- [ ] Búsqueda de texto dentro del libro
- [ ] Slider de progreso mejorado (saltar a posición dentro del capítulo)
- [ ] Gesto de brillo (deslizar lado izquierdo)
- [ ] Orientación de pantalla configurable (auto, portrait, landscape)

## Fase 4 — Features nuevos

- [ ] Anotaciones y highlights (subrayar + guardar notas en Room)
- [ ] TTS (text-to-speech) con controles de reproducción
- [ ] Diccionario integrado (tap en palabra → definición)
- [ ] Soporte PDF
- [ ] Estadísticas de lectura (tiempo leído, páginas por día, racha)
- [ ] Importar desde más fuentes (Open Library, Standard Ebooks, Internet Archive)

## Fase 5 — Play Store

- [ ] Crear cuenta de desarrollador en Google Play ($25)
- [x] Redactar política de privacidad
- [ ] Completar cuestionario de clasificación de contenido
- [ ] Preparar screenshots y ficha de la app (título, descripción, gráficos)
- [ ] Primer release en Play Store
- [ ] Configurar CI/CD para builds automáticos (GitHub Actions)
