Source

composer create-project drupal/recommended-project drupal
cd drupal
composer require drush/drush
composer require drupal/admin_toolbar
composer require drupal/pathauto
composer require drupal/devel
composer require drupal/migrate_plus
composer require drupal/migrate_tools
composer require drupal/migrate_source_csv
cd web/profiles
git clone git@github.com:makinacorpus/drupal-training-profile.git training_profile
cd training_profile
git submodule init modules/training_migrate_content
git submodule init modules/training_module
git submodule init modules/training_correction
git submodule init themes/training_theme
git submodule update --recursive --remote
