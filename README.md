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

Para configurar el UUID de drupal correr:
`ddev exec drush config-set system.site uuid 4c6a17a5-b5c2-4f3d-a4bf-346bd24620bd`

`ddev exec drush config-set system.site name  'Auriazules.com - La Vieja Guardia'`


Cambia tu carpeta de SYNC a:
```
if (defined('CONFIG_SYNC_DIRECTORY') && empty($config_directories[CONFIG_SYNC_DIRECTORY])) {
  $config_directories[CONFIG_SYNC_DIRECTORY] = 'sites/default/files/5432167890/sync';
}
elseif (empty($settings['config_sync_directory'])) {
  $settings['config_sync_directory'] = 'sites/default/files/5432167890/sync';
}
```
