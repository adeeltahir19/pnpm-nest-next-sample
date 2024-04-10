# README

## Tasks

### Backend

1. Setup `api` module with standard REST endpoints for `CRUD` operations (accepting both query strings and body data)
   1. Setup DB model (example in `api/src/user`) and DTO classes
   2. Link column in generated model with `user.model.ts` using sequelize foreign keys
   3. Add custom endpoint outside of standard CRUD
   4. Store all data using sqllite
   5. Create service using sequelize model methods for CRUD functions
2. Setup secondary `api` module with random `service`
3. Inject service in first generated module
4. Add correct `@nestjs/swagger` decorators on controller

### Frontend

1. Setup new page with components for CRUD operations
   1. Simple list, create, update and delete
   2. Use `swr` to call backend api (`axiosApi` const is ready for use as fetcher function)
   3. `react-hook-form` example for update
2. Generate new redux slice for persisting some data into the store during above ops

### Tests

1. Add unit tests to `api` module
2. Add E2E test to `api` module, using `supertest` and `expect` schemas (eg: `toMatchObject(schema)`)
3. Add frontend component test for one React component ensuring it renders correctly

&nbsp;
&nbsp;
&nbsp;
&nbsp;
&nbsp;

## Setup

```shell
nvm use
pnpm install
pnpm dev
```

## Local Development

- [Back Office](http://localhost:3000/)
- [Back Office API](http://localhost:4000/)
