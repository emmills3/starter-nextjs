# Starter NextJS Configuration

A starter setup for a basic NextJS app, includes basic packages for deployment and simple configurations.

**Basic configs:**
- jsconfig.json - Reset baseUrl to allow easy use of absolute paths
- .env - Basic, repo controlled config with public, non-sensitive environment data/keys/variables
- .env.development - Developement only .env file
- .env.production - Production only .env file
- .env.local - Non-repo controlled confif for sensitive environment data/keys/variables *(Must be created separately)*

**For server support:**
- pm2 (https://github.com/Unitech/pm2)
- cross-var (https://github.com/elijahmanor/cross-var)
- dotenv-cli (https://github.com/entropitor/dotenv-cli)

## Basic

Install packages: ```bash npm ci```
Run as development: ```npm run dev```
Create production build: ```npm run build```
Starting app in AWS Node environment (after building): ```pm2 restart [id]```  

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.js`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on 

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.
- [API routes](https://nextjs.org/docs/api-routes/introduction) - For app custom middleware layer
