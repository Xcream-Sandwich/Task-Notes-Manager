# 📝 Task & Notes Manager

A modern, responsive web application for managing your tasks and notes in one place. Built with cutting-edge technologies to provide a seamless user experience across all devices.

## ✨ Features

### 📝 To-Do List Management
- **Create Tasks**: Add new todos with title, description, and priority levels
- **Priority System**: Organize tasks with Low, Medium, and High priority levels
- **Task Status**: Mark tasks as complete or incomplete with interactive checkboxes
- **Task Filtering**: View all tasks, active tasks, or completed tasks
- **Edit & Delete**: Full CRUD operations for task management
- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices

### 📓 Notes Management
- **Create Notes**: Write notes with rich content and titles
- **Tag System**: Organize notes with customizable tags
- **Search Functionality**: Find notes instantly by searching title, content, or tags
- **Card Layout**: Beautiful grid layout that adapts to screen size
- **Full CRUD**: Complete create, read, update, and delete operations
- **Content Preview**: See note previews in the card view

### 🎨 User Experience
- **Dark/Light Theme**: Switch between themes with system preference detection
- **Responsive Design**: Mobile-first approach with adaptive layouts
- **Smooth Animations**: Delightful micro-interactions and transitions
- **Touch-Friendly**: Optimized for mobile devices with proper touch targets
- **Modern UI**: Clean, intuitive interface using shadcn/ui components

## 🚀 Technology Stack

### 🎯 Core Framework
- **⚡ Next.js 15** - React framework with App Router
- **📘 TypeScript 5** - Type-safe JavaScript development
- **🎨 Tailwind CSS 4** - Utility-first CSS framework

### 🧩 UI Components & Styling
- **🧩 shadcn/ui** - High-quality, accessible components
- **🎯 Lucide React** - Beautiful icon library
- **🌈 Framer Motion** - Smooth animations and transitions
- **🎨 Next Themes** - Dark/light mode support

### 📋 Forms & Validation
- **🎣 React Hook Form** - Performant form handling
- **✅ Zod** - TypeScript-first schema validation

### 🔄 State Management & Data Fetching
- **🐻 Zustand** - Simple state management
- **🔄 TanStack Query** - Server state management
- **🌐 Axios** - HTTP client for API requests

### 🗄️ Database & Backend
- **🗄️ Prisma** - Modern database ORM
- **💾 SQLite** - Lightweight database for local development

## 🎯 Why Choose This App?

- **🏎️ Fast & Responsive**: Optimized for performance across all devices
- **🎨 Beautiful UI**: Modern, clean interface with smooth interactions
- **🔒 Type Safe**: Full TypeScript implementation with validation
- **📱 Mobile First**: Designed to work perfectly on all screen sizes
- **🗄️ Data Persistent**: Reliable database storage with Prisma ORM
- **🌙 Theme Support**: Dark and light mode with system preference
- **🔍 Powerful Search**: Instant search across all notes and tags
- **📊 Task Organization**: Priority-based task management system

## 🚀 Quick Start

```bash
# Install dependencies
npm install

# Set up the database
npm run db:push

# Start development server
npm run dev

# Build for production
npm run build

# Start production server
npm start
```

Open [http://localhost:3000](http://localhost:3000) to see your application running.

## 📁 Project Structure

```
src/
├── app/                 # Next.js App Router pages and API routes
│   ├── api/            # API endpoints for todos and notes
│   └── page.tsx        # Main application page
├── components/          # Reusable React components
│   ├── ui/             # shadcn/ui components
│   ├── todo-section.tsx    # Todo management component
│   ├── notes-section.tsx   # Notes management component
│   ├── theme-toggle.tsx    # Theme switching component
│   └── theme-provider.tsx  # Theme provider wrapper
├── hooks/              # Custom React hooks
├── lib/                # Utility functions and configurations
│   ├── db.ts          # Database connection
│   ├── types.ts       # TypeScript type definitions
│   └── utils.ts       # Utility functions
└── prisma/             # Database schema and migrations
```

## 🎨 Available Features

### 📝 To-Do List Features
- **Task Creation**: Add tasks with title, description, and priority
- **Priority Levels**: Color-coded priority badges (Low, Medium, High)
- **Status Management**: Check/uncheck tasks to mark completion
- **Task Filtering**: Filter by All, Active, or Completed tasks
- **Inline Editing**: Edit tasks without leaving the main view
- **Bulk Operations**: Multiple task management capabilities

### 📓 Notes Features
- **Rich Content**: Create notes with titles and detailed content
- **Tag System**: Add multiple tags to organize notes
- **Instant Search**: Real-time search across titles, content, and tags
- **Card Layout**: Responsive grid layout with content previews
- **Tag Filtering**: Click tags to filter related notes
- **Content Management**: Full CRUD operations for notes

### 🎨 UI/UX Features
- **Theme Switching**: Toggle between light and dark modes
- **Responsive Design**: Adaptive layouts for all screen sizes
- **Smooth Animations**: Delightful transitions and micro-interactions
- **Touch Optimized**: Mobile-friendly interface elements
- **Loading States**: Skeleton loaders and progress indicators
- **Error Handling**: User-friendly error messages and recovery

## 🗄️ Database Schema

The application uses Prisma with SQLite and includes the following models:

### Todo Model
- `id` - Unique identifier
- `title` - Task title
- `description` - Optional task description
- `completed` - Completion status
- `priority` - Priority level (0: Low, 1: Medium, 2: High)
- `createdAt` - Creation timestamp
- `updatedAt` - Last update timestamp

### Note Model
- `id` - Unique identifier
- `title` - Note title
- `content` - Note content
- `tags` - JSON array of tags
- `createdAt` - Creation timestamp
- `updatedAt` - Last update timestamp

## 🔧 Development

### Database Operations
```bash
# Push schema changes to database
npm run db:push

# Generate Prisma client
npm run db:generate

# Create and run migrations
npm run db:migrate

# Reset database
npm run db:reset
```

### Code Quality
```bash
# Run linting
npm run lint
```

## 🚀 Deployment

The application is production-ready with:
- **Optimized Builds**: Automatic code splitting and optimization
- **Static Export**: Support for static hosting
- **Environment Variables**: Configurable for different environments
- **Error Handling**: Comprehensive error boundaries and logging

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

