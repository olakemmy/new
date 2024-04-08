# Next.js Application

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).


## Prerequisites

Before you begin, ensure you have met the following requirements:

- You have installed Node.js and npm/yarn.
- You have a MongoDB Atlas account.
- You have a Google account for Google OAuth.
- You have a Facebook account for Facebook OAuth.
- You have a Backblaze B2 Cloud Storage account.

## Setting Up .env File

Create a `.env` file in the root directory of your project and add the following environment variables:

```
GOOGLE_ID=your_google_id
FACEBOOK_CLIENT_ID=your_facebook_client_id
FACEBOOK_CLIENT_SECRET=your_facebook_client_secret
DB_NAME=your_database_name
URL=your_mongodb_connection_string
NEXTAUTH_SECRET=your_nextauth_secret
NEXT_PUBLIC_PROD_URI=your_production_graphql_endpoint
NEXT_PUBLIC_DEV_URI=your_development_graphql_endpoint
NEXT_PUBLIC_GOOGLE_CLIENT_ID=your_public_google_client_id
NEXT_PUBLIC_DEVE_URL=your_development_url
NEXT_PUBLIC_PRODU_URL=your_production_url
NEXT_PUBLIC_CLIENT_API_KEY=your_client_api_key
BACKBLAZE_APPLICATION_KEY_ID=your_backblaze_application_key_id
BACKBLAZE_APPLICATION_KEY=your_backblaze_application_key
BACKBLAZE_BUCKET_ID=your_backblaze_bucket_id

```

# Setting Up Environment Variables:

This Next.js app relies on several environment variables for configuration. Here's how you can obtain the necessary credentials:

## Google OAuth:

- Go to the Google Developer Console.
- Create a new project or select an existing one.
- Navigate to the "Credentials" tab and create OAuth 2.0 credentials.
- Copy the client ID and paste it into the GOOGLE_ID variable.
- Set the NEXT_PUBLIC_GOOGLE_CLIENT_ID variable with the same value.

## Facebook OAuth:

- Go to the Facebook Developers portal.
- Create a new app or select an existing one.
- Navigate to the "Settings" tab and copy the App ID and App Secret into the respective variables.

## MongoDB Atlas:

- If you don't already have a MongoDB Atlas account, sign up for one:
  - Go to MongoDB Atlas.
  - Create a new cluster and database.
  - Copy the connection string and set it as the value for the URL variable in your .env file.

## NextAuth:

- Generate a secure secret for NextAuth:
  - Generate a random string and set it as the value for the NEXTAUTH_SECRET variable.

## Next.js API URIs:

- Set the NEXT_PUBLIC_PROD_URI and NEXT_PUBLIC_DEV_URI variables with the respective GraphQL API URIs for production and development environments.

## Backblaze:

- Obtain the Backblaze B2 Cloud Storage credentials:
  - Sign in to your Backblaze account or sign up for one if you don't have it.
  - Navigate to the B2 Cloud Storage section.
  - Create a new application key, and copy the Application Key ID and Application Key values into the respective variables.
  - Set the BACKBLAZE_BUCKET_ID variable with the ID of the bucket you want to use.

# Running the Application:

- Install dependencies using `npm install` or `yarn install`.
- Start the development server using `npm run dev` or `yarn dev`.


Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.


## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.
