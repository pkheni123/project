# Project Bolt

A modern web application built with React, TypeScript, and Supabase for authentication.

## Features

- User authentication (sign up, sign in, sign out)
- Protected routes
- Modern UI with Tailwind CSS
- TypeScript for type safety
- Vite for fast development and building

## Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- A Supabase account and project

## Setup

1. Clone the repository:
```bash
git clone <repository-url>
cd project-bolt
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file in the root directory with your Supabase credentials:
```
VITE_SUPABASE_URL=your-supabase-project-url
VITE_SUPABASE_ANON_KEY=your-supabase-anon-key
```

You can find these values in your Supabase project settings.

## Development

To start the development server:

```bash
npm run dev
```

The application will be available at `http://localhost:5173`.

## Building for Production

To create a production build:

```bash
npm run build
```

The built files will be in the `dist` directory.

## Project Structure

- `src/components/` - Reusable UI components
- `src/contexts/` - React contexts (including authentication)
- `src/pages/` - Application pages/routes
- `src/lib/` - Utility functions and configurations

## Technologies Used

- React
- TypeScript
- Vite
- Tailwind CSS
- Supabase
- React Router DOM

## License

MIT 