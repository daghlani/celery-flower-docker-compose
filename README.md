# Flower Docker Compose
 This is a docker-compose repo to use [This](https://github.com/mher/flower/tree/master) project (docker version). This is a way to monitor your tasks on celery python projects.
## Usage

  - create a environment file:

    ```bash
    cp sample.env .env
    ```



  - edit .env:
    ```bash
    vi .env
    ```
  - This is a sample of environment file. change it according your broker (redis). if your broker is anything else of redis, you can change the broker url in compose file.
    ```bash
    REDIS_PASSWORD=pass
    REDIS_HOST=host
    REDIS_PORT=12345
    REDIS_CELERY_DB=15
    ```
    Content:

    - REDIS_PASSWORD: password of redis
    - REDIS_HOST: host of redis
    - REDIS_PORT: redis port
    - REDIS_CELERY_DB: database of your celery in redis



  - then save environment file and run docker-compose file by this command:
    ```bash
    docker-compose up -d

    ```

>  For more information you can read original docs in [This](om/mher/flower/tree/master) repository
