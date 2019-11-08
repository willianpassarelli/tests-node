## TESTS NODE

Tests NODE with Jest and Supertest

### Run tests config (package.json) in windows

```
  "scripts": {
    ...
    "pretest": "set NODE_ENV=test && sequelize db:migrate",
    "test": "set NODE_ENV=test && jest",
    "posttest": "set NODE_ENV=test && sequelize db:migrate:undo:all"
  }
```

### Run tests config (package.json) in mac

```
  "scripts": {
    ...
    "pretest": "NODE_ENV=test sequelize db:migrate",
    "test": "NODE_ENV=test jest",
    "posttest": "NODE_ENV=test sequelize db:migrate:undo:all"
  }
```
