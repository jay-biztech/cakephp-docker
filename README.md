# Setup CakePHP using docker
1. Copy Dockerfile and docker-compose.yml files to your project root directory.

2. Build the image of the container
   ```sh
   docker-compose build
   ```

3. Start the service
   ```sh
   docker-compose up
   ```

4. Stop the service
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



