# Dependencies

```bash
npm install --save-dev prisma

```

### create a tsconfig.json file

# Initialize Prisma with database

```bash
npx prisma init --datasource-provider postgresql

```

# Define your model in schema.prisma 

# Migrate your schema to database

```bash
npx prisma migrate dev --name init

```

# Create Prisma Client

```bash
npm i @prisma/client
```

# Manually generate your client

```bash
npx prisma generate
```

### open your script.ts and write 

```bash
import { PrismaClient } from "@prisma/client";
const prisma = new PrismaClient();

```

### or if you are using javascript, write

```bash
const {PrismaClient} = require('@prisma/client');
const prisma = new PrismaClient();
```

# After making any changes to the schema 
```bash
npx prisma migrate dev --name init
npx prisma generate

```