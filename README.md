# PruebaAI - Ruby on Rails

Proyecto de prueba desarrollado en Ruby on Rails con vistas y rutas configuradas. Una aplicación web completa con navegación entre páginas (Inicio, Productos y About).

## Descripción

PruebaAI es una aplicación web moderna construida con Rails que demuestra conceptos fundamentales del framework como controladores, vistas, rutas y estilos CSS básicos.

## Requisitos Previos

Antes de comenzar, asegúrate de tener instalado lo siguiente:

- **Ruby**: versión 3.2.0 o superior
- **Rails**: versión 7.0.0 o superior
- **SQLite3**: para la base de datos (incluido por defecto en Rails)
- **Node.js**: versión 14.0 o superior (requerido para Asset Pipeline)
- **Bundler**: para gestionar dependencias de gemas

## Instalación

### 1. Clonar el repositorio

```bash
git clone https://github.com/Gibson2/PruebaAI-RubyonRails.git
cd PruebaAI-RubyonRails
```

### 2. Instalar dependencias

```bash
bundle install
```

### 3. Crear la base de datos

```bash
rails db:create
rails db:migrate
```

## Uso

### Iniciar el servidor de desarrollo

```bash
rails server
```

O de forma más corta:

```bash
rails s
```

La aplicación estará disponible en `http://localhost:3000`

### Rutas disponibles

- **Inicio**: `/home/index` o `/` (página principal con menú de navegación)
- **Productos**: `/products/index` (página de productos)
- **About**: `/about/index` (página de información)

## Estructura del Proyecto

```
PruebaAI/
├── app/
│   ├── controllers/          # Controladores de la aplicación
│   │   ├── home_controller.rb
│   │   ├── products_controller.rb
│   │   └── about_controller.rb
│   ├── views/                # Vistas (templates HTML/ERB)
│   │   ├── home/
│   │   ├── products/
│   │   └── about/
│   ├── models/               # Modelos de datos
│   ├── helpers/              # Funciones auxiliares
│   └── assets/               # Assets (CSS, imágenes, JavaScript)
├── config/
│   ├── routes.rb             # Configuración de rutas
│   └── database.yml          # Configuración de base de datos
├── db/
│   ├── migrate/              # Migraciones de base de datos
│   └── seeds.rb              # Datos de prueba
├── test/                     # Tests y especificaciones
├── Gemfile                   # Dependencias del proyecto
└── README.md                 # Este archivo
```

## Dependencias principales

- **rails**: Framework web principal
- **sqlite3**: Adaptador de base de datos
- **puma**: Servidor web
- **sprockets-rails**: Asset pipeline
- **importmap-rails**: Gestor de módulos JavaScript

Ver `Gemfile` para la lista completa de dependencias.

## Desarrollo

### Ejecutar tests

```bash
rails test
```

### Generar un nuevo controlador

```bash
rails generate controller NombreControlador accion1 accion2
```

### Generar un nuevo modelo

```bash
rails generate model NombreModelo atributo1:tipo atributo2:tipo
```

## Contribución

Para contribuir a este proyecto:

1. Crea una rama para tu funcionalidad (`git checkout -b feature/AmazingFeature`)
2. Realiza tus cambios (`git commit -m 'Add some AmazingFeature'`)
3. Envía tus cambios (`git push origin feature/AmazingFeature`)
4. Abre un Pull Request

## Licencia

Este proyecto está bajo la licencia MIT. Ver el archivo `LICENSE` para más detalles.

## Autor

**Gibson2** - [GitHub Profile](https://github.com/Gibson2)

## Soporte

Si encuentras problemas o tienes preguntas, por favor abre un issue en el [repositorio](https://github.com/Gibson2/PruebaAI-RubyonRails/issues).

## Changelog

### Versión 1.0.0 (2026-05-05)
- Creación inicial del proyecto
- Configuración de controladores (Home, Products, About)
- Creación de vistas con menú de navegación
- Estilos CSS básicos para botones
- Sincronización con GitHub
