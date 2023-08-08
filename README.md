npx prisma db push

npx ts-node --require tsconfig-paths/register prisma/seed.ts

or

npx prisma db seed

user: kody
password: twixrox

SESSION_SECRET

```bash
openssl rand -base64 32
```

## Fly.io

```bash
flyctl auth signup
flyctl launch

flyctl secrets set SESSION_SECRET=<something>
flyctl secrets set DATABASE_URL=<data base url>

npx prisma migrate dev

# Optional
npx prisma db seed

flyctl deploy
```
