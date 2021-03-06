# Build a FULL STACK App w/ TypeScript, Next JS, Apollo - Task Management App Part 1 (of 3) [2022]
https://www.youtube.com/watch?v=64PU6zWUTG8&ab_channel=webdecoded



Code: https://github.com/judygab/Jira-Asana-Clone


- Next.js as the React framework
- Apollo Server as the GraphQL server
- Nexus for constructing the GraphQL schema
- Apollo Client as the GraphQL client
- Prisma as the ORM for migrations and database access
- PostgreSQL as the database
- Sendgrid as mail server & passwordless authentication
- TypeScript as the programming language


1. Create Next App
```
  npx create-next-app@latest --ts
```

2. Setup Prisma
```
  npm i prisma @prisma/client -D

  npx prisma init
```

3. Setup PostgreSql on Heroku
```
  1. Create new app
  2. Resource -> Add-ons Select Heroku Posgres
  3. get the crednetials
```

4. Setup PrismaClient
Create db    
```
npx prisma db push  
```

Open prisma GUI and add data
```
npx prisma studio
```

Crete lib/prisma.ts hold a global instance of PrismaClient


5. Setup GraphQL
nexus for schema generation
```
  npm i graphql nexus
```
Use Next.js api routes to create GraphQL endpoint
/pages/api


 