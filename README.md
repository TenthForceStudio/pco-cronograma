# Cronograma — Politécnico Cristo Obrero

Cronograma interactivo de la **Plataforma de Gestión Escolar** del Politécnico Cristo Obrero.

## 🌐 Ver en línea

Una vez publicado en GitHub Pages estará disponible en:
```
https://<tu-usuario>.github.io/<nombre-del-repo>/
```

---

## 🚀 Cómo publicar en GitHub Pages

### Opción A — Automático con GitHub Actions (recomendado)

1. Crear un repositorio nuevo en GitHub (ej: `pco-cronograma`)
2. Subir todos los archivos de esta carpeta al repositorio
3. Ir a **Settings → Pages**
4. En **Source** seleccionar: `GitHub Actions`
5. Hacer push a `main` — el workflow se ejecuta automáticamente
6. En 1-2 minutos el sitio estará publicado

### Opción B — Manual desde rama

1. Crear repositorio en GitHub
2. Subir archivos
3. Ir a **Settings → Pages**
4. En **Source** seleccionar: `Deploy from a branch`
5. Seleccionar rama `main` y carpeta `/ (root)`
6. Guardar — GitHub Pages publica automáticamente

---

## 📁 Estructura del proyecto

```
/
├── index.html          ← Aplicación completa (todo en un archivo)
├── README.md           ← Este archivo
└── .github/
    └── workflows/
        └── deploy.yml  ← Workflow de auto-deploy a GitHub Pages
```

> El cronograma es una **Single Page Application** sin dependencias externas ni build step.
> Solo HTML + CSS + JavaScript vanilla. Se abre directo en cualquier navegador.

---

## ✏️ Cómo actualizar tareas o fechas

Abre `index.html` y busca la sección `// ── DATA ──` en el JavaScript.

Cada tarea tiene esta estructura:
```js
{
  name:    'Nombre de la tarea',
  area:    'backend',          // coord | backend | frontend | db | security | media | general
  color:   'c-backend',        // clase CSS de color del área
  start:   2,                  // semana de inicio (0=sem1, 1=sem2, 2=sem3, 3=sem4)
  dur:     1,                  // duración en semanas (0.5 = media semana)
  persons: 'Wilfredo · Kemil', // responsables visibles en tooltip
  detail:  'Descripción...'    // detalle en tooltip al pasar el mouse
}
```

---

## 🛠️ Tecnologías

- HTML5 + CSS3 + JavaScript ES6 vanilla
- Google Fonts: DM Serif Display + DM Mono + Outfit
- Sin frameworks, sin npm, sin build step
- Compatible con todos los navegadores modernos

---

## 👥 Equipo

| Área | Integrantes |
|------|-------------|
| Coordinación | Yeliana Díaz |
| Backend | Wilfredo · Christopher · Kemil |
| Frontend | Alvely · Josue · Leury |
| Base de Datos | Yeliana · Mariana |
| Ciberseguridad | Jeison |
| Multimedia | Elixandra |

---

*Politécnico Cristo Obrero — Versión 1.0 — Abril 2026*
