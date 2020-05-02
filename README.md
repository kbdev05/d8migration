# kushald8migration


Run docker build -t drupal8migration:latest
docker-compose up -d

docker-compose exec drupal bash -c 'drush site:install minimal --db-url="mysql://drupal:$DRUPAL_DATABASE_PASSWORD@$DRUPAL_DATABASE_HOST/drupal" --site-name="D8 migration" -y'
