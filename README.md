# NestJS Boilerplate

>Hey there! Are you looking for an example NestJS project? Or perhaps you want to start a project without wasting time on implementing authentication, setting up connections to MongoDB and Redis, adding logging and Swagger? Maybe you just want to explore new code concepts. Well, you've come to the right place - welcome to my repository!

>This repository serves as my boilerplate project, which I use as a foundation for my new projects to save time.

### Includes;

- E2E tests
- Authentication (JWT tokens)
- Daily logging with Winston
- Useful decorators
- Interceptor for response transformation and logging
- Error handling filter
- Caching with Redis
- Handling race conditions
- MongoDB integration
- Docker configuration

## Running the Project

```bash
$ cd docker
$ docker-compose up 
```
The project will be accessible at http://localhost:3050.


## Stopping the Project

```bash
$ docker-compose down
```

### Accessing API Documentation
>http://localhost:3050/api

### Testing
> I utilize Jest for E2E testing. You can find the test scripts in the 'test' folder.
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

### License
> There is no any license for this project. You are free to use and modify the code as you see fit.