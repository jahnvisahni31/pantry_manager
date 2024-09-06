# Pantry Tracker

A web application to help you keep track of your pantry items, built with Next.js and Firebase.

## Features

- User authentication (sign up, login, logout)
- Add, edit, and delete pantry items
- Real-time updates using Firebase Realtime Database
- Responsive design for mobile and desktop

## Technologies Used

- [Next.js](https://nextjs.org/) - React framework for server-side rendering and static site generation
- [Firebase](https://firebase.google.com/) - Backend-as-a-Service (BaaS) for authentication and database
- [React](https://reactjs.org/) - JavaScript library for building user interfaces
- [Tailwind CSS](https://tailwindcss.com/) - Utility-first CSS framework

## Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (v14 or later)
- npm (v6 or later)

## Getting Started

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/pantry-tracker.git
   cd pantry-tracker
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Set up Firebase:
   - Create a new Firebase project at [https://console.firebase.google.com/](https://console.firebase.google.com/)
   - Enable Authentication and Realtime Database in your Firebase project
   - Create a web app in your Firebase project and copy the configuration
   - Create a `.env.local` file in the root directory and add your Firebase configuration:
     ```
     NEXT_PUBLIC_FIREBASE_API_KEY=your_api_key
     NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_auth_domain
     NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
     NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_storage_bucket
     NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_messaging_sender_id
     NEXT_PUBLIC_FIREBASE_APP_ID=your_app_id
     ```

4. Run the development server:
   ```
   npm run dev
   ```

5. Open [http://localhost:3000](http://localhost:3000) in your browser to see the application.

## Folder Structure

```
pantry-tracker/
├── components/
│   ├── Layout.js
│   ├── PantryItem.js
│   └── PantryList.js
├── pages/
│   ├── api/
│   ├── _app.js
│   ├── index.js
│   ├── login.js
│   └── signup.js
├── styles/
│   └── globals.css
├── utils/
│   └── firebase.js
├── .env.local
├── .gitignore
├── next.config.js
├── package.json
└── README.md
```

## Deployment

To deploy your Pantry Tracker application, you can use [Vercel](https://vercel.com/), which is optimized for Next.js projects:

1. Push your code to a GitHub repository
2. Connect your GitHub account to Vercel
3. Import your repository and deploy

Alternatively, you can deploy to other platforms that support Next.js applications.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the [MIT License](LICENSE).
