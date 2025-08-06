# Portfolio Application

## Overview

This is a sophisticated dual-theme cinematic portfolio website for Vishal Singh, a USC Computer Science master's student. The application features two distinct modes: a modern corporate Professional theme with warm beige backgrounds and 3D code line animations, and a Dragon Ball theme with parallax scrolling and animations, switchable via a "Transform" button. The portfolio includes a comprehensive Personal page with artwork gallery, LinkedIn post previews, real GitHub projects showcase, and a fully functional contact form with real email delivery.

## User Preferences

- **Communication style**: Simple, everyday language
- **Theme approach**: Dual-theme system (Professional/Dragon Ball) with smooth transitions
- **Contact functionality**: Real email integration only, no mock data
- **Branding**: USC prominence with official logos throughout
- **Social presence**: LinkedIn (vishalsingh148), GitHub (14vishal), contact email (vishal14899@gmail.com)

## Recent Progress (August 2025)

- ✅ Implemented dual-theme system with conditional scroll animations
- ✅ Fixed scroll offsets (Professional: 800px, Dragon Ball: 0px) 
- ✅ Updated introduction text to concise grad school journey
- ✅ Configured Personal page to open directly to Recent section
- ✅ Updated all social media links with real URLs
- ✅ Implemented complete contact form with SendGrid integration
- ✅ Added SendGrid API key to project secrets
- ✅ Added "Check out Personal" animated indicator to navigation
- ✅ Implemented comprehensive copyright protection system
- ✅ Fixed Python and Unity logo visibility with proper asset imports
- ✅ Updated Projects section with real GitHub projects
- ⚠️ **Pending**: SendGrid sender verification needed for email delivery

## System Architecture

### Frontend Architecture
The frontend is built with React and TypeScript, utilizing a component-based architecture with modern UI patterns:

- **React 18** with TypeScript for type-safe component development
- **Vite** as the build tool and development server for fast hot module replacement
- **Wouter** for lightweight client-side routing instead of React Router
- **Framer Motion** for smooth animations and transitions throughout the portfolio
- **Tailwind CSS** with CSS variables for consistent theming and responsive design
- **shadcn/ui** component library providing pre-built, accessible UI components

The application follows a single-page application (SPA) pattern with smooth scrolling navigation between sections. Components are organized into logical directories with clear separation of concerns between UI components, pages, and utility functions.

### Backend Architecture
The backend follows a RESTful API design pattern built with Express.js:

- **Express.js** server with TypeScript for type-safe API development
- **Modular routing system** with centralized route registration
- **Storage abstraction layer** using an interface pattern that supports both in-memory storage and database implementations
- **Session handling** configured for PostgreSQL with connect-pg-simple
- **Middleware architecture** for request logging, error handling, and CORS

The server is designed to be easily extensible with additional API endpoints and can switch between different storage implementations without changing business logic.

### Data Storage Solutions
The application is configured for PostgreSQL database integration:

- **Drizzle ORM** for type-safe database operations and migrations
- **PostgreSQL** as the primary database (configured via DATABASE_URL environment variable)
- **Neon Database** integration for serverless PostgreSQL hosting
- **Database schema** defined with user management capabilities
- **In-memory fallback storage** for development and testing scenarios

The storage layer uses an interface pattern allowing easy switching between different implementations while maintaining consistent API contracts.

### Styling and Design System
The design system is built around a cohesive visual language:

- **Tailwind CSS** with custom configuration for design tokens
- **CSS variables** for theme consistency and potential dark mode support
- **Component variants** using class-variance-authority for consistent styling patterns
- **Responsive design** with mobile-first approach
- **Custom animations** with Framer Motion for enhanced user experience

### Development and Build Pipeline
The project uses modern development tooling:

- **TypeScript** throughout the stack for type safety
- **ESBuild** for fast production builds
- **Vite** for development with hot module replacement
- **Path aliases** for clean import statements
- **Shared types** between frontend and backend via the shared directory

## External Dependencies

### Communication Services
- **SendGrid** - Email delivery service for contact form (API key configured in secrets)
- **LinkedIn API** - For post previews and professional content integration

### Database and Hosting
- **Neon Database** - Serverless PostgreSQL database hosting
- **Replit** - Development and deployment platform with integrated tooling
- **Google Cloud Storage** - Object storage for artwork and assets

### UI and Animation Libraries
- **Radix UI** - Comprehensive set of accessible, unstyled UI primitives
- **Framer Motion** - Production-ready motion library for React animations
- **Lucide React** - Modern icon library with consistent design
- **React Icons** - Popular icon library for social media and brand icons

### Development Tools
- **TanStack Query** - Server state management for data fetching and caching
- **React Hook Form** - Performant forms library with validation support
- **Zod** - TypeScript-first schema validation library
- **date-fns** - Modern JavaScript date utility library

### Typography and Fonts
- **Google Fonts** - Inter and Poppins font families for modern typography
- Custom font loading with preconnect optimization for performance

The application is designed to be easily deployable to various platforms while maintaining consistent functionality across different environments.