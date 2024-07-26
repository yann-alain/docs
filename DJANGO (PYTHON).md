1. Comprendre que les vues sont ce que verront l'utilisateur.
2. Les urls vont créer le chemin.
3. `__init__.py` and `apps.py` establish the project structure and application configuration.
- `asgi.py` defines the entry point for web servers to handle requests.
- `admin.py` provides a user-friendly interface for managing model data.
- `models.py` defines the data models that represent your database schema.
- The `migrations` folder in a Django app plays a crucial role in managing database schema changes. It stores migration files, which are essentially instructions for Django to apply updates to the database structure. These migrations ensure that your database remains consistent with the evolving models defined in your Django application
- Static files and templates are fundamental components of Django web development. Static files provide the styling, interactivity, and multimedia elements, while templates define the structure and dynamic content integration for user-facing web pages. Together, they enable the creation of rich, interactive, and data-driven web applications using Django.

La commande `makemigrations` est un outil indispensable pour gérer les évolutions de votre base de données dans un projet Django. Elle vous permet de maintenir une cohérence entre vos modèles et votre base de données, et de suivre les changements au fil du temps.

- **Exécutez `makemigrations` régulièrement** après avoir modifié vos modèles.
- **Utilisez `migrate`** pour appliquer les migrations à votre base de données.

python manage.py makemigrations (faire la migration vers une nouvelle vue)
>python manage.py sqlmigrate polls 0001 (pour voir ma base de données)
>python manage.py migrate
>python manage.py shell
>