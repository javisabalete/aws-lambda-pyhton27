# aws-lambda-pyhton27
Run and build your aws lambda applications written in python.

## Usage

1. Copy files to your python project.

2. Add your requeriments to requeriments.txt

3. Build and start containers.

    ```bash
    docker-compose up --build
    ```

On finish, your project will have been packaged in ```proj.zip```, ready to upload in aws lambda.

## Execute command on the container

    docker run --rm -v $(pwd):/root/proj --env-file=.env $(docker build -q .) HERE_YOUR_COMMAND
  
