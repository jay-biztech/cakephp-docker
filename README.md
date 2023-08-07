# Setup CakePHP using docker
1. Copy Dockerfile and docker-compose.yml files to your project root directory.

2. Make sure you update the database in config/app.php and MYSQL_DATABASE in docker-compose.yml.

3. Build the image of the container
   ```sh
   docker-compose build
   ```

4. Start the service
   ```sh
   docker-compose up
   ```

5. Stop the service
   ```sh
   docker-compose down
   ```

### You can run below command inside the container
1. Install the composer
   ```sh
   docker-compose run cakephp composer install --no-interaction
   ```

2. Migration 
   ```sh
   docker-compose run cakephp bin/cake migrations migrate
   ```
   
3. Stop service with volume
   ```sh
   docker-compose down -v
   ```



