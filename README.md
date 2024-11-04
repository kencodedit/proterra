
# Proterra Application
This is an application which allows users to properly manage and change status of projects.

###  Technology Stack Used

- **Frontend**: Next.js, Tailwind CSS, Redux Toolkit, Redux Toolkit Query, Material UI Data Grid
- **Backend**: Node.js with Express, Prisma (PostgreSQL ORM)
- **Database**: PostgreSQL, managed with PgAdmin
- **Cloud**: AWS EC2, AWS RDS, AWS API Gateway, AWS Amplify, AWS S3, AWS Lambda, AWS Cognito


### Prerequisites

Ensure you have these tools installed:

- Git
- Node.js
- npm (Node Package Manager)
- PostgreSQL ([download](https://www.postgresql.org/download/))
- PgAdmin ([download](https://www.pgadmin.org/download/))

### Installation Steps

1. Install dependencies in both client and server:
   `cd portal`
   `npm i`
   `cd ..`
   `cd backend-server`
   `npm i`

2. Set up the database:
   `npx prisma generate`
   `npx prisma migrate dev --name init`
   `npm run seed`

3. Configure environment variables:

- `.env` for backend-server settings (PORT, DATABASE_URL)
- `.env.local` for portal settings (NEXT_PUBLIC_API_BASE_URL)

4. Run the project
   `npm run dev`