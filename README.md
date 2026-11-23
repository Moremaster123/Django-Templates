# Plantillas de Django

Plantillas del e-commerce con herencia y fragmentos reutilizables. Forma parte de la serie de tareas del proyecto e-commerce de la profesión Full Stack Python de EBAC. Cada repositorio guarda el proyecto como quedó al terminar ese tema; la versión final es [e-commerce-completo](https://github.com/Moremaster123/e-commerce-completo).

## Tecnologías

- Python y Django 6.1
- Bootstrap 5.3
- SQLite

## Cómo están organizadas las plantillas

- `templates/base.html`: estructura general con los bloques `title`, `content` y `extra_js`.
- `templates/includes/`: barra de navegación, pie de página, mensajes y encabezado de página.
- `product/`: lista de productos con una tarjeta reutilizable (`product_card.html`) y página de detalle.
- `sales/`: panel de ventas con tarjetas de estadísticas y lista de pedidos.
- `accounts/register.html`: formulario de registro.

## Rutas

| Ruta | Página |
|---|---|
| `/products/` | Lista de productos |
| `/products/<id>/` | Detalle de un producto |
| `/accounts/register/` | Registro |
| `/sales/` | Panel de ventas (solo administradores) |

## Cómo ejecutarlo

```bash
python -m venv venv
venv\Scripts\activate        # en Linux o macOS: source venv/bin/activate
pip install django
python manage.py migrate
python manage.py createsuperuser
python manage.py crear_ventas
python manage.py runserver
```

Abre `http://127.0.0.1:8000/`. Te redirige a la lista de productos.

## Autor

Juan Carlos González Herrera · [LinkedIn](https://www.linkedin.com/in/juan-carlos-desarrollador-web) · [Portafolio](https://moremaster123.github.io)
