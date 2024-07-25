# Latihan membuat aplikasi blog - Medium Clone


#### 1. Inisial komit

        new file:   .gitignore
        new file:   readme.md

#### 2. Membuat venv

        (medium-cln) λ python -m venv venv312413 --promp medium-cln
        (medium-cln) λ venv312413\Scripts\activate.bat
        (medium-cln) λ pip install -r requirements.txt

        modified:   .gitignore
        modified:   readme.md
        new file:   requirements.txt

#### 3. Menginisiasi proyek

        new file:   config/__init__.py
        new file:   config/asgi.py
        new file:   config/settings.py
        new file:   config/urls.py
        new file:   config/wsgi.py
        new file:   manage.py

#### 4. Membuat app page, home view

        modified:   config/settings.py
        modified:   config/urls.py
        new file:   page/__init__.py
        new file:   page/admin.py
        new file:   page/apps.py
        new file:   page/migrations/__init__.py
        new file:   page/models.py
        new file:   page/templates/page/home_page.html
        new file:   page/tests.py
        new file:   page/views.py
        modified:   readme.md