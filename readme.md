# Latihan membuat aplikasi blog - Medium Clone
https://github.com/gurnitha/2024-practice-project-4-medium-clone

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

### 5. Mengisi template, dan load static files pada homepage

        modified:   config/settings.py
        modified:   page/templates/page/home_page.html
        new file:   static_files/css/bootstrap.min.css
        new file:   static_files/css/bootstrap.min.css.map
        new file:   static_files/css/style.css
        new file:   static_files/js/bootstrap.bundle.min.js
        new file:   static_files/js/bootstrap.bundle.min.js.map
        new file:   templates/core/base.html
        new file:   templates/core/navbar.html

        :)

#### 6. Membuat app blog dan user_profile, dan login page

        new file:   blog/__init__.py
        new file:   blog/admin.py
        new file:   blog/apps.py
        new file:   blog/migrations/__init__.py
        new file:   blog/models.py
        new file:   blog/tests.py
        new file:   blog/views.py
        modified:   config/settings.py
        modified:   config/urls.py
        new file:   templates/core/base_without_navbar.html
        new file:   user_profile/__init__.py
        new file:   user_profile/admin.py
        new file:   user_profile/apps.py
        new file:   user_profile/migrations/__init__.py
        new file:   user_profile/models.py
        new file:   user_profile/templates/user_profile/login.html
        new file:   user_profile/tests.py
        new file:   user_profile/urls.py
        new file:   user_profile/views.py

        (medium-cln) λ python manage.py makemigrations
        No changes detected

        E:\_WORKSPACE\2024\django\BLOG\TURKI-Hakan Yalçınkaya\practice_project_4_medium_clone(master)
        (medium-cln) λ python manage.py migrate
        Operations to perform:
          Apply all migrations: admin, auth, contenttypes, sessions
        Running migrations:
          Applying contenttypes.0001_initial... OK
          Applying auth.0001_initial... OK
          Applying admin.0001_initial... OK
          Applying admin.0002_logentry_remove_auto_add... OK
          Applying admin.0003_logentry_add_action_flag_choices... OK
          Applying contenttypes.0002_remove_content_type_name... OK
          Applying auth.0002_alter_permission_name_max_length... OK
          Applying auth.0003_alter_user_email_max_length... OK
          Applying auth.0004_alter_user_username_opts... OK
          Applying auth.0005_alter_user_last_login_null... OK
          Applying auth.0006_require_contenttypes_0002... OK
          Applying auth.0007_alter_validators_add_error_messages... OK
          Applying auth.0008_alter_user_username_max_length... OK
          Applying auth.0009_alter_user_last_name_max_length... OK
          Applying auth.0010_alter_group_name_max_length... OK
          Applying auth.0011_update_proxy_permissions... OK
          Applying auth.0012_alter_user_first_name_max_length... OK
          Applying sessions.0001_initial... OK

        E:\_WORKSPACE\2024\django\BLOG\TURKI-Hakan Yalçınkaya\practice_project_4_medium_clone(master)
        (medium-cln) λ python manage.py createsuperuser
        Username (leave blank to use 'ing'): superuser
        Email address: superuser@mail.com
        Password:
        Password (again):
        The password is too similar to the email address.
        Bypass password validation and create user anyway? [y/N]: y
        Superuser created successfully.

        NOTE:

        Belum bisa login.

#### 7. Membuat logik pada login_view

        modified:   config/settings.py
        modified:   user_profile/views.py

        NOTE:

        Belum bisa login.

#### 8. Django-Messages-Framework

        modified:   templates/core/base.html
        new file:   templates/core/messages.html
        modified:   user_profile/views.py

        NOTE:

        1. Belum bisa login.
        2. Message tidak muncul.

#### 9. Modified Django-Messages-Framework

        modified:   readme.md
        modified:   templates/core/messages.html

        NOTE:

        1. Berhasil login dan redirect ke homepage.
        2. Message sudah muncul.

        :)

#### 10. Logout

        modified:   readme.md
        modified:   user_profile/urls.py
        modified:   user_profile/views.py

        NOTE:

        1. Logout :)
        2. Login (:

#### 11. Login: added more conditionals on login_view

        modified:   templates/core/base_without_navbar.html
        modified:   user_profile/views.py

#### 12. Creating the Sign-Up-Register-Page

        modified:   config/settings.py
        modified:   readme.md
        modified:   templates/core/navbar.html
        new file:   user_profile/templates/user_profile/register.html
        modified:   user_profile/urls.py
        modified:   user_profile/views.py

#### 13. Creating-User-Profile-Model-Structure

        modified:   user_profile/models.py
        modified:   user_profile/templates/user_profile/register.html
        modified:   user_profile/views.py