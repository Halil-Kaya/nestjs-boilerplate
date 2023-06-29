# NestJS Boilerplate

> Hey ✋Are you looking an example nestjs project? or you want to make a project, but you don't want to waste time with
> implementing authentication, mongo and redis connection adding logging and swagger? or you just want to see new code
> consepts. welcome to my repo.

> This repo is my boilerplate project. I'm building my new projects from this repo to don't waste time.

### Includes;

-   E2E tests
-   Authentication (Jwt token)
-   daily logging with winston
-   usefully decorators
-   interceptor to transform response and logging
-   filter to error handling
-   caching with redis
-   handling race condition
-   mongo
-   docker

## To run project

```bash
$ cd docker
$ docker-compose up 
```
it will up on http://localhost:3050

## To stop project

```bash
$ docker-compose down
```

### To reach Api document
>http://localhost:3050/api

### Testing

> I'm using jest for e2e testing. you can find my test scripts in 'test' folder.

```bash
test
├── api
│   ├── auth
│   │   └── sign-in.test.ts
│   └── user
│       └── user-create.test.ts
├── common
│   ├── auth.helper.ts
│   ├── db
│   │   ├── index.ts
│   │   ├── mongo.helper.ts
│   │   └── redis.helper.ts
│   ├── helper.ts
│   ├── index.ts
│   └── user.helper.ts
├── jest-e2e.json
├── test-config.ts
└── test-setup.ts
```

## To run tests

```bash
$ npm run test
```