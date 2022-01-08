# DjangoAuthJWTFlow


remember to enable CORS support with Django Rest using django-cors-header

run  pip install django-cors-headers

If the installation is done, go to your settings.py file and add the package in INSTALLED_APPS and the middleware.
INSTALLED_APPS = [
    ...
    'corsheaders',
    ...
]

MIDDLEWARE = [
    ...
    'corsheaders.middleware.CorsMiddleware',
    'django.middleware.common.CommonMiddleware',
    ...
]
And add these lines at the end of the settings.py file.
CORS_ALLOWED_ORIGINS = [
    "http://localhost:3000",
    "http://127.0.0.1:3000"
] for local machine testing
