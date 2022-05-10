## Description
- This is only a template for future projects.

## Docker Setup
```
docker volume rm $(docker volume ls -q)
docker system prune
docker compose up --build -d
docker compose logs -f
```

## Note
- Since we are using the docker virtual environment, we run the script inside
the docker. Below are the following commands:
```
  docker-compose exec frontend npm run dev
    - Running the localhost:3000 server.

  docker-compose exec frontend npm run format
    - Applying the prettier.

  docker-compose exec frontend npm run lint
    - Applying the linter.

  docker-compose exec frontend npm run test
    - Applying the Jest testing.
```

- For ease of convenience in development, you can use the VSCode extensions for docker or the Docker desktop.

## Recordings
https://user-images.githubusercontent.com/87509953/167068939-7d3e28d6-9cf0-4582-b60e-6f5e8d0b0ffd.mp4
