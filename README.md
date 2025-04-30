# The Calendar

A modern web application with authentication and 2FA built with React, TypeScript, and Supabase.

## Quick Start Guide

### Prerequisites

1. Node.js (v14 or higher) - [Download here](https://nodejs.org/)
2. A Supabase account (free) - [Sign up here](https://supabase.com/)

### Setting up Supabase

1. Go to [Supabase](https://supabase.com/) and create a new account or sign in
2. Create a new project
3. Once your project is ready, go to Project Settings > API
4. You'll need two values from this page:
   - Project URL (anon/public)
   - anon/public key

### Running the Application

1. Unzip the project files to a directory of your choice
2. Open a terminal/command prompt and navigate to the project directory
3. Create a new file named `.env` in the project root directory
4. Add the following to your `.env` file (replace with your Supabase values):
   ```
   VITE_SUPABASE_URL=your-project-url
   VITE_SUPABASE_ANON_KEY=your-anon-key
   ```
5. Install dependencies:
   ```bash
   npm install
   ```
6. Start the development server:
   ```bash
   npm run dev
   ```
7. Open your browser and navigate to `http://localhost:5173` (or the URL shown in your terminal)

### Test Credentials

For testing the application:
- Any email format will work for registration
- Use code `123456` for 2FA verification (this is a demo implementation)

### Features

- User authentication (sign up, sign in, sign out)
- Two-factor authentication (demo)
- Password reset flow (demo)
- Protected routes
- Modern UI with Tailwind CSS
- TypeScript for type safety

### Troubleshooting

1. If you see "Module not found" errors:
   - Make sure you've run `npm install`
   - Try deleting the `node_modules` folder and running `npm install` again

2. If you see environment variable errors:
   - Make sure you've created the `.env` file
   - Verify the variable names match exactly: `VITE_SUPABASE_URL` and `VITE_SUPABASE_ANON_KEY`
   - Make sure there are no spaces around the `=` in the `.env` file

3. If the application can't connect to Supabase:
   - Verify your Supabase project is active
   - Check that your URL and anon key are correct
   - Make sure you're using the anon/public key, not the service role key

### Project Structure

- `src/components/` - Reusable UI components
- `src/contexts/` - React contexts (including authentication)
- `src/pages/` - Application pages/routes
- `src/lib/` - Utility functions and configurations

### Technologies Used

- React 18
- TypeScript
- Vite
- Tailwind CSS
- Supabase
- React Router DOM

### Note

This is a demo application with simplified authentication flows. In a production environment, you would want to:
- Implement proper email verification
- Use real 2FA with TOTP or SMS
- Add proper password reset functionality
- Implement rate limiting
- Add additional security measures

## License

MIT 