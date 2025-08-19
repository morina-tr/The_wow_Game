# Overview

This is a sophisticated 3D First Person Shooter (FPS) game built with React Three Fiber that combines advanced gaming features with C++ programming education. Players engage in immersive FPS gameplay with ESP (wall hack) and aimbot capabilities while learning C++ concepts through AI-powered educational content. The game features realistic soldier enemies, multiple weapon systems, tactical AI behavior powered by Gemini API, and atmospheric 3D environments. The project showcases modern web game development with full-stack architecture using Express.js backend, PostgreSQL database integration via Drizzle ORM, and comprehensive UI components.

## Recent Achievements (January 2025)
- ✅ Transformed from puzzle game to full-featured FPS
- ✅ Implemented ESP system for seeing enemies through walls
- ✅ Added aimbot with automatic target acquisition
- ✅ Created 4 weapon system (pistol, rifle, sniper, shotgun)
- ✅ Integrated Gemini AI for enemy tactical behavior
- ✅ Built realistic soldier models with damage system
- ✅ Enhanced graphics with fog, shadows, and 3D environment objects
- ✅ Prepared project for GitHub publication with comprehensive documentation

## Project Status: Ready for GitHub Publication
The project is now a complete, feature-rich 3D FPS game ready for open-source distribution.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture

The frontend is built using React with TypeScript and leverages React Three Fiber for 3D graphics. The application uses a component-based architecture with:

- **3D Game Engine**: React Three Fiber (@react-three/fiber) provides the WebGL rendering layer
- **3D Components**: Individual game objects (Player, Level, Goal, Switch, PuzzleBlock) are separate components
- **State Management**: Zustand stores handle game state, puzzle logic, and audio management
- **UI Framework**: Radix UI components with Tailwind CSS for styling
- **Control System**: Keyboard controls using @react-three/drei KeyboardControls

## Backend Architecture

The backend uses Express.js with TypeScript and follows a modular structure:

- **Express Server**: Handles HTTP requests and serves the React application
- **Storage Interface**: Abstracted storage layer with in-memory implementation (ready for database integration)
- **Route Registration**: Centralized route management system
- **Development Mode**: Vite integration for hot module replacement during development

## State Management

Three primary Zustand stores manage application state:

- **useGame**: Controls overall game phases (ready, playing, ended)
- **usePuzzle**: Manages level data, player position, and puzzle mechanics
- **useAudio**: Handles sound effects and background music with mute functionality

## Data Storage

- **Database**: PostgreSQL configured through Drizzle ORM
- **Schema**: User management with username/password authentication structure
- **Development Storage**: In-memory storage implementation for rapid prototyping
- **Migration System**: Drizzle Kit handles database schema changes

## 3D Graphics and Physics

- **Rendering**: Three.js via React Three Fiber for WebGL-based 3D graphics
- **Collision Detection**: Custom AABB (Axis-Aligned Bounding Box) collision system
- **Camera Controls**: Orbit controls for 3D scene navigation
- **Lighting**: Directional lighting with shadow casting enabled

## Build System

- **Development**: Vite for fast development builds and HMR
- **Production**: esbuild for server bundling, Vite for client assets
- **TypeScript**: Full type checking across client, server, and shared code
- **Asset Handling**: Support for 3D models (.gltf, .glb) and audio files

# External Dependencies

## Core Frameworks
- **React Three Fiber**: 3D rendering and WebGL integration
- **Express.js**: Web server framework
- **React**: UI framework with TypeScript support

## Database and ORM
- **PostgreSQL**: Primary database (configured via DATABASE_URL)
- **Drizzle ORM**: Type-safe database operations and migrations
- **Neon Database**: Serverless PostgreSQL provider

## UI and Styling
- **Radix UI**: Comprehensive component library for accessibility
- **Tailwind CSS**: Utility-first CSS framework
- **class-variance-authority**: Component variant management

## Development Tools
- **Vite**: Build tool and development server
- **esbuild**: Fast JavaScript bundler for production
- **TypeScript**: Static type checking
- **PostCSS**: CSS processing with Autoprefixer

## Game-Specific Libraries
- **@react-three/drei**: React Three Fiber utilities and helpers
- **@react-three/postprocessing**: Post-processing effects
- **Zustand**: Lightweight state management
- **TanStack Query**: Data fetching and caching

## AI Integration
- **Google Gemini API**: Generates educational C++ content for completed levels
- **Environment Variables**: VITE_GEMINI_API_KEY for API access

## Audio System
- **Web Audio API**: Native browser audio handling
- **HTML5 Audio**: Background music and sound effects
- **Audio Assets**: MP3, OGG, and WAV format support