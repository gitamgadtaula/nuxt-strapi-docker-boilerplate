# Docker, Nuxt3, Strapi and Mysql

### We have option to run all 3 stacks in docker but we may want to only run the database in container and run both frontend and strapi locally because it is fast

Running the database

```
docker-compose pull
docker-compose up db

```

Running the frontend

```
cd frontend
yarn install
yarn dev
```

Running the backend

```
cd backend
yarn install
yarn develop
```
