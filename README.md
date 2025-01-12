# AdonisJS 6 + Vue 3 Starter

A full-featured starter template combining [AdonisJS 6](https://docs.adonisjs.com/guides/introduction) and [Vue 3](https://vuejs.org/) with server-side rendering (SSR).

> Inspired by [Adocasts Jumpstart](https://github.com/adocasts/jumpstart) by [Tom Gobich](https://github.com/tomgobich) and Tom's work.

## Features

- **Full-stack Framework**: Built with [AdonisJS 6](https://adonisjs.com/) ([Documentation](https://docs.adonisjs.com/guides/introduction)) and [Vue 3](https://vuejs.org/)
- **Server-side Rendering**: Configured with Inertia.js for SSR support
- **UI Components**: Integrated [shadcn-vue](https://shadcn-vue.com/) components
- **Authentication**:
  - Session-based authentication
  - Google OAuth integration
  - Password reset functionality
  - Login/Register flows
- **Type Safety**: Full TypeScript support
- **Modern Styling**: TailwindCSS with CSS variables

## Getting Started

1. Clone the repository
2. Copy `.env.example` to `.env` and configure your environment variables
3. Install dependencies:

    ```sh
    npm install
    ```

4. Start the development server:

    ```sh
    npm run dev
    ```

## Project Structure

```md
.
├── app/ # Server-side application code
│ ├── controllers/ # HTTP request handlers
│ ├── middleware/ # Custom middleware
│ └── models/ # Database models
├── config/ # Application configuration
├── database/ # Database migrations and seeders
├── inertia/ # Inertia server configuration
├── public/ # Static assets
├── resources/ # Frontend assets
│ ├── css/ # Global styles
│ ├── js/ # Vue components and utilities
│ └── views/ # Inertia page components
├── start/ # Application bootstrapping
└── tests/ # Test files
```

## Authentication Setup

1. Configure Google OAuth:

   - Visit [Google Cloud Console](https://console.cloud.google.com)
   - Create a new project
   - Enable Google OAuth API
   - Create credentials (OAuth client ID)
   - Set authorized redirect URI to: `http://localhost:3333/auth/google/callback`
   - Add credentials to `.env`:

     ```env
     GOOGLE_CLIENT_ID=your_client_id
     GOOGLE_CLIENT_SECRET=your_client_secret
     ```

## Frontend Development

- Components are in `inertia/components`
- Pages are in `inertia/pages`
- Customize UI components directly from shadcn vue

## Development

### Commands
