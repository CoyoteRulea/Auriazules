# Auriazules

Para instalar este codigo siga los pasos de instalación de DDEV
https://www.drupal.org/docs/official_docs/en/_local_development_guide.html

En caso de tener y previamente instalado, corra los siguientes pasos:
```
composer create-project drupal/recommended-project auriazules`

cd auriazules

ddev config --docroot web --project-name $SITE_NAME --project-type drupal9

ddev start
```

Posteriormente para clonar el repo:
```
git init

git remote add origin https://github.com/CoyoteRulea/auriazules.git

git pull origin main
```
