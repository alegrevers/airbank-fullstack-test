# Airbank FullStack Test

## API Setup
```
cd backend
yarn install
cp .env.example .env
npm start
```

### API database migration
```
sudo -i -u postgres
psql
DROP DATABASE IF EXISTS airbank
CREATE DATABASE airbank
npx prisma migrate dev --name init
npx prisma migrate reset --force
npx prisma db seed
```

## Frontend setup
```
cd front
yarn install
cp .env.example .env
yarn serve
```
