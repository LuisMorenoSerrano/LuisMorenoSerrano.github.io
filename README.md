# LuisMorenoSerrano.github.io

🌐 **Personal Portfolio & Project Showcase**

Este es mi portfolio digital construido con Jekyll y hospedado en GitHub Pages. Muestra mis proyectos principales de desarrollo en múltiples lenguajes de programación y tecnologías.

## 🚀 Ver el Sitio

**Producción:** [https://LuisMorenoSerrano.github.io](https://LuisMorenoSerrano.github.io)

**Versión Español:** [https://LuisMorenoSerrano.github.io/es](https://LuisMorenoSerrano.github.io/es)

## 🛠️ Tecnologías

- **Jekyll 3.10.0** - Generador de sitios estáticos
- **jekyll-theme-yat** - Tema moderno y responsivo
- **GitHub Actions** - CI/CD automático para deployment
- **HTML/CSS/Liquid** - Frontend con templates Liquid
- **YAML** - Gestión de datos de proyectos

## 📦 Desarrollo Local

### Requisitos Previos

- **Ruby** 3.2+
- **Bundler**
- **Git**

### Instalación en Ubuntu/Linux

1. **Instalar Ruby y dependencias:**

   ```bash
   sudo apt install ruby-full build-essential zlib1g-dev
   ```

2. **Configurar gems en directorio de usuario:**

   ```bash
   echo '# Ruby gems configuration' >> ~/.bashrc
   echo 'export GEM_HOME="$HOME/.gems"' >> ~/.bashrc
   echo 'export PATH="$HOME/.gems/bin:$PATH"' >> ~/.bashrc
   source ~/.bashrc
   ```

3. **Instalar Bundler:**

   ```bash
   gem install bundler
   ```

4. **Clonar el repositorio:**

   ```bash
   git clone https://github.com/LuisMorenoSerrano/LuisMorenoSerrano.github.io.git
   cd LuisMorenoSerrano.github.io
   ```

5. **Instalar dependencias del proyecto:**

   ```bash
   bundle install
   ```

6. **Ejecutar servidor de desarrollo:**

   ```bash
   bundle exec jekyll serve
   ```

7. **Abrir en navegador:**
   - Accede a [http://localhost:4000](http://localhost:4000)
   - Los cambios se recargan automáticamente (excepto `_config.yml`)

### Comandos Útiles

```bash
# Build del sitio (output en _site/)
bundle exec jekyll build

# Servidor con drafts
bundle exec jekyll serve --drafts

# Limpiar archivos generados
bundle exec jekyll clean

# Ver versión de Jekyll
bundle exec jekyll --version
```

## 📁 Estructura del Proyecto

```txt
.
├── _data/              # Datos YAML (proyectos, configuración)
│   └── projects.yml    # Lista de proyectos del portfolio
├── _includes/          # Componentes reutilizables
│   └── project-cards.html
├── _layouts/           # Plantillas de página
│   └── portfolio.html
├── assets/             # Recursos estáticos
│   └── css/
│       └── portfolio.css
├── .github/            # CI/CD
│   └── workflows/
│       └── jekyll.yml  # GitHub Actions workflow
├── index.markdown      # Página principal (EN)
├── es.markdown         # Página principal (ES)
├── _config.yml         # Configuración Jekyll
├── Gemfile             # Dependencias Ruby
└── README.md           # Este archivo
```

## ✏️ Añadir Proyectos

Los proyectos se gestionan centralizadamente en `_data/projects.yml`:

```yaml
- name: "Nombre del Proyecto"
  slug: "proyecto-slug"
  description:
    en: "English description"
    es: "Descripción en español"
  technologies:
    - Tech1
    - Tech2
  github_url: "https://github.com/usuario/repo"
  status: "active"  # complete, in-development, learning, active, maintained, optimized
  icon: "🚀"
  featured: true    # Mostrar primero
```

Los cambios en este archivo se reflejan automáticamente en ambas versiones (EN/ES) sin necesidad de editar el HTML.

## 🎨 Personalización CSS

Los estilos personalizados están en `assets/css/portfolio.css`. El diseño incluye:

- ✅ Hero section con gradiente
- ✅ Grid responsivo de proyectos
- ✅ Cards con hover effects
- ✅ Badges de tecnologías
- ✅ Secciones de habilidades y contacto
- ✅ Variables CSS para temas

## 🚀 Deployment

El sitio se despliega automáticamente mediante GitHub Actions:

1. **Push a `main`** → Trigger automático del workflow
2. **Build con Jekyll** → Genera sitio estático
3. **Deploy a GitHub Pages** → Publicación automática

### Configurar GitHub Pages

1. Ve a repositorio → Settings → Pages
2. Source: **GitHub Actions**
3. El workflow `.github/workflows/jekyll.yml` se encarga del resto

## 📝 Licencia

Este proyecto es personal. El código está disponible para referencia educativa.

## 📬 Contacto

- **GitHub:** [@LuisMorenoSerrano](https://github.com/LuisMorenoSerrano)
- **Email:** [lmoreno.serrano@gmail.com](mailto:lmoreno.serrano@gmail.com)

---

**Última actualización:** Febrero 2026
