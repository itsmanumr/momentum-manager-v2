# Plan de Migración de Branding: Evolution API → MomentumChat

## 📋 Resumen Ejecutivo

Este documento detalla todas las modificaciones necesarias para cambiar completamente el branding del repositorio de **Evolution API** a **MomentumChat**.

---

## 🎯 Áreas de Cambio

### 1. **Archivos de Configuración del Proyecto**

#### 1.1 `package.json`
**Cambios necesarios:**
- `name`: `"evolution-manager"` → `"momentumchat-manager"` o `"momentum-chat-manager"`
- `description`: `"Modern web interface for Evolution API management"` → `"Modern web interface for MomentumChat management"`
- `keywords`: Remover `"evolution-api"`, agregar `"momentumchat"`, `"momentum-chat"`
- `homepage`: Actualizar URL del repositorio
- `repository.url`: Actualizar URL del repositorio
- `bugs.url`: Actualizar URL de issues
- `author.name`: `"Evolution API Team"` → `"MomentumChat Team"`
- `author.email`: `"contato@evolution-api.com"` → Email de MomentumChat
- `author.url`: `"https://evolution-api.com"` → URL de MomentumChat
- `contributors`: Actualizar información del equipo

#### 1.2 `index.html`
**Cambios necesarios:**
- `<title>`: `"Evolution Manager"` → `"MomentumChat Manager"`
- `favicon`: Cambiar URL de `https://evolution-api.com/files/evo/favicon.svg` → Logo de MomentumChat

#### 1.3 `docker-compose.yml`
**Cambios necesarios:**
- `services.evolution-manager`: Renombrar a `momentumchat-manager` o `momentum-chat-manager`
- `container_name`: `"evolution-manager-v2"` → `"momentumchat-manager-v2"`
- `networks.evolution-network`: Renombrar a `momentumchat-network`
- Comentarios sobre Evolution API: Actualizar o remover

---

### 2. **Archivos de Documentación**

#### 2.1 `README.md`
**Cambios necesarios:**
- Título: `"Evolution Manager v2"` → `"MomentumChat Manager v2"`
- Logo: Cambiar referencia de `evolution-logo.png` → Logo de MomentumChat
- Subtítulo: `"Modern Web Interface for Evolution API Management"` → `"Modern Web Interface for MomentumChat Management"`
- Enlaces de demo/documentación/comunidad: Actualizar URLs
- Sección "About": 
  - `"Evolution Manager v2"` → `"MomentumChat Manager v2"`
  - Referencias a Evolution API → MomentumChat
- Sección "Features": Actualizar descripciones
- Sección "Installation": Actualizar comandos y referencias
- Sección "Configuration": Actualizar variables de entorno
- Sección "API Integration": Actualizar referencias
- Sección "Support": Actualizar emails y URLs
- Footer: `"Made with ❤️ by the Evolution API Team"` → `"Made with ❤️ by the MomentumChat Team"`
- Enlaces de GitHub: Actualizar URLs del repositorio

#### 2.2 `CHANGELOG.md`
**Cambios necesarios:**
- Título: `"Evolution Manager v2"` → `"MomentumChat Manager v2"`
- Todas las referencias a "Evolution Manager" → "MomentumChat Manager"
- Referencias a "Evolution API" → "MomentumChat"

#### 2.3 `SECURITY.md`
**Cambios necesarios:**
- Título y referencias: `"Evolution Manager"` → `"MomentumChat Manager"`
- Email de contacto: `contato@evolution-api.com` → Email de MomentumChat
- URL de GitHub: Actualizar repositorio
- Firma: `"Evolution Manager Security Team"` → `"MomentumChat Security Team"`

#### 2.4 `LICENSE`
**Cambios necesarios:**
- Título: `"Evolution Manager License"` → `"MomentumChat Manager License"`
- Todas las referencias a "Evolution Manager" → "MomentumChat Manager"
- Referencias a "Evolution API" → "MomentumChat"
- Email de contacto: Actualizar
- Copyright: `"© 2025 Evolution API"` → `"© 2025 MomentumChat"`

---

### 3. **Archivos de Código Fuente - Componentes UI**

#### 3.1 `src/components/header.tsx`
**Cambios necesarios:**
- Línea 34: Cambiar URLs de logos de Evolution API → Logos de MomentumChat
  - `"https://evolution-api.com/files/evo/evolution-logo-white.svg"` → Logo oscuro MomentumChat
  - `"https://evolution-api.com/files/evo/evolution-logo.svg"` → Logo claro MomentumChat
- Línea 39: `"/assets/images/evolution-logo.png"` → `"/assets/images/momentumchat-logo.png"`

#### 3.2 `src/components/footer.tsx`
**Cambios necesarios:**
- Líneas 21-34: Actualizar todos los enlaces:
  - `"https://evolution-api.com/discord"` → Discord de MomentumChat
  - `"https://evolution-api.com/postman"` → Postman de MomentumChat (si aplica)
  - `"https://github.com/EvolutionAPI/evolution-api"` → Repositorio de MomentumChat
  - `"https://doc.evolution-api.com"` → Documentación de MomentumChat

#### 3.3 `src/components/sidebar.tsx`
**Cambios necesarios:**
- Línea 124: `"https://doc.evolution-api.com"` → Documentación de MomentumChat
- Línea 131: `"https://evolution-api.com/postman"` → Postman de MomentumChat
- Línea 137: `"https://evolution-api.com/discord"` → Discord de MomentumChat
- Línea 143: `"https://evolution-api.com/suporte-pro"` → Soporte de MomentumChat

---

### 4. **Archivos de Código Fuente - Páginas**

#### 4.1 `src/pages/Home.tsx`
**Cambios necesarios:**
- Líneas 24-25: URLs de logos → Logos de MomentumChat
- Línea 25: `alt="Evolution API Logo"` → `alt="MomentumChat Logo"`
- Líneas 40-42: URLs de logos → Logos de MomentumChat
- Línea 42: `alt="Evolution Manager Logo"` → `alt="MomentumChat Manager Logo"`
- Línea 47: `"Evolution Manager v2"` → `"MomentumChat Manager v2"`
- Línea 50: `"Modern web interface for Evolution API management"` → `"Modern web interface for MomentumChat management"`
- Línea 62: `"Welcome to Evolution Manager"` → `"Welcome to MomentumChat Manager"`
- Línea 65: `"A powerful, modern dashboard for managing your WhatsApp API instances with Evolution API"` → `"A powerful, modern dashboard for managing your WhatsApp API instances with MomentumChat"`
- Línea 89: `"Get help, contribute, or learn more about Evolution API"` → `"Get help, contribute, or learn more about MomentumChat"`
- Línea 95: URL de GitHub → Repositorio de MomentumChat
- Línea 108: `"https://evolution-api.com"` → URL de MomentumChat
- Línea 121: `"mailto:contato@evolution-api.com"` → Email de MomentumChat
- Línea 136: `"© 2025 Evolution API. Licensed under Apache 2.0 with Evolution API custom conditions."` → `"© 2025 MomentumChat. Licensed under Apache 2.0 with MomentumChat custom conditions."`

#### 4.2 `src/pages/Login/index.tsx`
**Cambios necesarios:**
- Línea 74: URLs de logos → Logos de MomentumChat
- El título viene de traducciones (ver sección de traducciones)

---

### 5. **Archivos de Traducción (i18n)**

#### 5.1 `src/translate/languages/en-US.json`
**Cambios necesarios:**
- Línea 85: `"evolutionBot": "Evolution Bot"` → `"evolutionBot": "MomentumChat Bot"` (o mantener técnico si es nombre de API)
- Línea 100: `"title": "Evolution Manager"` → `"title": "MomentumChat Manager"`
- Línea 126: `"evolution": "Evolution"` → `"evolution": "MomentumChat"` (si es visible al usuario)
- Líneas 1157-1285: Sección `evolutionBot`:
  - `"title": "Evolution Bot"` → `"title": "MomentumChat Bot"`
  - Todos los mensajes que mencionen "Evolution Bot" → "MomentumChat Bot"
- Revisar todas las referencias a "Evolution" en textos visibles al usuario

#### 5.2 `src/translate/languages/es-ES.json`
**Cambios necesarios:**
- Mismos cambios que `en-US.json` pero en español
- `"Evolution Manager"` → `"MomentumChat Manager"`
- `"Bot Evolution"` → `"Bot MomentumChat"` (o mantener técnico según contexto)

#### 5.3 `src/translate/languages/pt-BR.json`
**Cambios necesarios:**
- Mismos cambios que `en-US.json` pero en portugués
- `"Evolution Manager"` → `"MomentumChat Manager"`
- `"Bot Evolution"` → `"Bot MomentumChat"` (o mantener técnico según contexto)

#### 5.4 `src/translate/languages/fr-FR.json`
**Cambios necesarios:**
- Mismos cambios que `en-US.json` pero en francés
- `"Evolution Manager"` → `"MomentumChat Manager"`
- `"Bots Evolution"` → `"Bots MomentumChat"` (o mantener técnico según contexto)

**Nota importante sobre traducciones:**
- Los nombres técnicos de tipos/interfaces (como `EvolutionBot` en código) pueden mantenerse si son parte de la API backend
- Solo cambiar textos visibles al usuario final
- Revisar contexto: si "Evolution Bot" es un nombre de producto vs nombre técnico

---

### 6. **Recursos Estáticos**

#### 6.1 `public/assets/images/evolution-logo.png`
**Acción requerida:**
- **REEMPLAZAR** el archivo con el logo de MomentumChat
- Renombrar a `momentumchat-logo.png` o mantener nombre según preferencia
- Actualizar todas las referencias en código

#### 6.2 Logos SVG (URLs externas)
**Acción requerida:**
- Obtener logos de MomentumChat en formato SVG (claro y oscuro)
- Subir a servidor propio o incluir en `public/assets/images/`
- Actualizar todas las URLs en código

---

### 7. **Nombres Técnicos vs Branding**

#### 7.1 Tipos e Interfaces TypeScript
**Decisión requerida:**
- `src/types/evolution.types.ts`: 
  - ¿Mantener nombre del archivo? (puede ser `momentumchat.types.ts`)
  - Tipos como `EvolutionBot`: ¿Mantener si es parte de la API backend?
- Si la API backend sigue usando "Evolution", mantener nombres técnicos
- Si la API backend también cambia, actualizar nombres

#### 7.2 Rutas y Paths
**Revisar:**
- `src/routes/index.tsx`: Rutas como `/evolutionBot` pueden mantenerse si son parte de la API
- Evaluar si cambiar rutas afecta compatibilidad con backend

#### 7.3 Nombres de Carpetas/Archivos
**Opcional:**
- `src/pages/instance/EvolutionBot/`: ¿Renombrar carpeta?
- `src/lib/queries/evolutionBot/`: ¿Renombrar carpeta?
- Considerar impacto en imports y compatibilidad

---

### 8. **Variables de Entorno y Configuración**

#### 8.1 Variables de Entorno (`.env.example` si existe)
**Cambios sugeridos:**
- `VITE_APP_NAME`: `"Evolution Manager"` → `"MomentumChat Manager"`
- `VITE_EVOLUTION_API_URL`: ¿Renombrar a `VITE_MOMENTUMCHAT_API_URL`?
- Revisar todas las variables que contengan "EVOLUTION"

#### 8.2 Comentarios en código
**Revisar:**
- Buscar comentarios que mencionen "Evolution API" o "Evolution Manager"
- Actualizar según contexto

---

## 📝 Checklist de Implementación

### Fase 1: Configuración Base
- [ ] Actualizar `package.json`
- [ ] Actualizar `index.html`
- [ ] Actualizar `docker-compose.yml`
- [ ] Reemplazar logos en `public/assets/images/`

### Fase 2: Documentación
- [ ] Actualizar `README.md`
- [ ] Actualizar `CHANGELOG.md`
- [ ] Actualizar `SECURITY.md`
- [ ] Actualizar `LICENSE`

### Fase 3: Componentes UI
- [ ] Actualizar `src/components/header.tsx`
- [ ] Actualizar `src/components/footer.tsx`
- [ ] Actualizar `src/components/sidebar.tsx`

### Fase 4: Páginas
- [ ] Actualizar `src/pages/Home.tsx`
- [ ] Actualizar `src/pages/Login/index.tsx`

### Fase 5: Traducciones
- [ ] Actualizar `src/translate/languages/en-US.json`
- [ ] Actualizar `src/translate/languages/es-ES.json`
- [ ] Actualizar `src/translate/languages/pt-BR.json`
- [ ] Actualizar `src/translate/languages/fr-FR.json`

### Fase 6: Recursos y Assets
- [ ] Obtener/subir logos de MomentumChat (SVG claro y oscuro)
- [ ] Reemplazar `evolution-logo.png`
- [ ] Actualizar todas las referencias a logos

### Fase 7: Limpieza y Verificación
- [ ] Buscar referencias restantes con `grep -r "evolution" --ignore-case`
- [ ] Buscar referencias restantes con `grep -r "evolution-api" --ignore-case`
- [ ] Verificar que no queden URLs de evolution-api.com
- [ ] Verificar que no queden emails de evolution-api.com
- [ ] Probar build: `npm run build`
- [ ] Probar en desarrollo: `npm run dev`
- [ ] Verificar todas las páginas visualmente

---

## ⚠️ Consideraciones Importantes

### 1. Compatibilidad con Backend API
- Si el backend sigue usando "Evolution API", mantener nombres técnicos en:
  - Tipos TypeScript
  - Rutas de API
  - Nombres de endpoints
- Solo cambiar branding visible al usuario

### 2. URLs y Enlaces Externos
- Decidir nuevas URLs para:
  - Documentación
  - Discord/Comunidad
  - Postman Collection
  - Soporte Premium
  - Website oficial
  - Repositorio GitHub

### 3. Emails de Contacto
- Definir nuevos emails para:
  - Contacto general
  - Soporte
  - Seguridad
  - Licencias comerciales

### 4. Logos y Assets
- Obtener logos en formatos:
  - PNG (para favicon y fallbacks)
  - SVG claro (para modo claro)
  - SVG oscuro (para modo oscuro)
  - Tamaños: favicon (16x16, 32x32), header (altura ~32px), home (altura ~40px)

### 5. Nombres de Producto
- Decidir naming convention:
  - "MomentumChat" (una palabra)
  - "Momentum Chat" (dos palabras)
  - "MomentumChat Manager" vs "MomentumChat Dashboard"

---

## 🔍 Búsquedas para Verificación Final

```bash
# Buscar todas las referencias a "evolution" (case insensitive)
grep -r "evolution" --ignore-case --exclude-dir=node_modules --exclude-dir=.git

# Buscar URLs de evolution-api.com
grep -r "evolution-api.com" --exclude-dir=node_modules --exclude-dir=.git

# Buscar emails de evolution-api.com
grep -r "evolution-api.com" --exclude-dir=node_modules --exclude-dir=.git

# Buscar "Evolution API" o "Evolution Manager"
grep -r "Evolution \(API\|Manager\)" --exclude-dir=node_modules --exclude-dir=.git
```

---

## 📊 Estadísticas Estimadas

- **Archivos a modificar**: ~25-30 archivos
- **Líneas de código afectadas**: ~200-300 líneas
- **Archivos de traducción**: 4 archivos (4 idiomas)
- **Recursos a reemplazar**: 1+ logos/imágenes
- **Tiempo estimado**: 4-6 horas de trabajo

---

## ✅ Criterios de Éxito

1. ✅ No hay referencias visibles a "Evolution API" en la UI
2. ✅ Todos los logos muestran branding de MomentumChat
3. ✅ Todas las URLs apuntan a recursos de MomentumChat
4. ✅ Todos los emails son de dominio MomentumChat
5. ✅ Documentación actualizada completamente
6. ✅ Build exitoso sin errores
7. ✅ Aplicación funciona correctamente en desarrollo y producción

---

**Última actualización**: [Fecha]
**Responsable**: [Nombre]
**Estado**: Planificación

