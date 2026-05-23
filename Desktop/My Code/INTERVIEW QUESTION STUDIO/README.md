<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />
</div>

# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/91e0bbb4-c07b-4f5e-aaec-5797bb1574db

## Run Locally

**Prerequisites:** Node.js

1. Install dependencies:
   `npm install`
2. Create a local `.env.local` or `.env` file and add:
   ```
   GEMINI_API_KEY=your_gemini_api_key_here
   ```
   This file is ignored by Git thanks to `.gitignore`.
3. Run the app:
   `npm run dev`

## Deploy to Vercel

On Vercel, do not store your API key in source control. Instead:

1. Open your Vercel project settings.
2. Add an environment variable named `GEMINI_API_KEY` with your secret key.
3. Deploy the project.

The server reads `process.env.GEMINI_API_KEY` at runtime, so the key remains server-side only.
 