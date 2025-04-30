# Chat AI UI

A modern Vue 3 application for interacting with an AI chatbot, built with TypeScript, Vite, and Pinia for state management.

## Features

- 🚀 Lightning-fast with Vite's modern build tooling
- 💬 Real-time chat interface with AI responses
- 👤 User management and authentication
- 📱 Responsive design with Tailwind CSS
- 🔄 Persistent state with Pinia store

## Tech Stack

- **Frontend Framework**: Vue 3 with Composition API
- **Build Tool**: Vite
- **Language**: TypeScript
- **State Management**: Pinia with persistence
- **Routing**: Vue Router
- **API Communication**: Axios
- **Styling**: Tailwind CSS

## Project Structure

```
src/
├── components/     # Reusable Vue components
│   ├── ChatInput.vue
│   └── Header.vue
├── hooks/          # Custom hooks including API functionality
│   └── api.ts      # Axios instance and API utilities
├── router/         # Vue Router configuration
│   └── index.ts
├── stores/         # Pinia state management
│   ├── chat.ts     # Chat interactions and history
│   └── user.ts     # User authentication and profile
├── views/          # Page components
│   ├── ChatView.vue
│   └── HomeView.vue
└── assets/         # Static assets
```

## Getting Started

### Prerequisites

- Node.js (v16+)
- npm or yarn

### Installation

1. Clone the repository:

   ```bash
   git clone <repository-url>
   cd chat-ai-ui
   ```

2. Install dependencies:

   ```bash
   npm install
   # or
   yarn
   ```

3. Create a `.env` file in the root directory with the following variables:
   ```
   VITE_API_URL=<your-backend-api-url>
   ```

### Development

```bash
npm run dev
# or
yarn dev
```

This will start the development server at `http://localhost:5173` (default).

### Build for Production

```bash
npm run build
# or
yarn build
```

The build artifacts will be stored in the `dist/` directory.

### Preview Production Build

```bash
npm run preview
# or
yarn preview
```

## API Integration

The application communicates with a backend API using Axios. API endpoints include:

- `/register-user` - User registration
- `/get-messages` - Retrieve chat history
- `/chat` - Send messages to the AI and receive responses

## Contributing

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/amazing-feature`
3. Commit your changes: `git commit -m 'Add some amazing feature'`
4. Push to the branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
