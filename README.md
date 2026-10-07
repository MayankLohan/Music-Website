# Spotify Clone - React Music Player

A responsive Spotify-inspired music streaming frontend built with React.js, Vite, JavaScript, and Tailwind CSS.

This project recreates the core visual experience of a modern music streaming application, including a Spotify-style sidebar, navigation bar, playlists and music cards, category filters, and a browser-based music player.

> **Project scope:** This is a frontend-only project. It does not currently include a backend, database, user authentication, Spotify API integration, or cloud-based music streaming.

---

## Features

### Music Player
- Browser-based audio playback using local music assets.
- Play/pause functionality.
- Previous and next song controls.
- Shuffle and repeat controls.
- Current song information and artwork.
- Playback progress bar.
- Current playback time and total duration.
- Player controls designed to remain usable across screen sizes.

### Home / Browse Interface
- Spotify-inspired dark interface.
- Featured charts section.
- Today's biggest hits / music recommendations.
- Music cards containing album artwork, title, and description.
- Category filters such as All, Music, and Podcast.
- Playlist/album information section.

### Sidebar
- Home navigation.
- Search navigation.
- Your Library section.
- Create Playlist card.
- Podcast discovery card.
- Responsive behavior for smaller screens.

### Navigation Bar
- Previous and next navigation buttons.
- Explore Premium button.
- Install App button.
- User profile indicator.
- Category filter buttons.

### Responsive Design
The interface uses Tailwind CSS responsive utilities to adapt the layout to different viewport sizes.

The application is designed for:
- Desktop
- Laptop
- Tablet
- Smaller screen sizes

---

## Technology Stack

| Technology | Purpose |
|---|---|
| React.js | Component-based frontend development |
| JavaScript | Application logic |
| Tailwind CSS | Styling and responsive UI |
| Vite | Development server and build tool |
| HTML5 | Application structure |
| CSS | Base styling |
| ESLint | Code quality and linting |
| npm | Package management |

---

## Project Structure

```text
song-player/
│
├── public/
│
├── src/
│   ├── assets/
│   │   └── assets.js
│   │
│   ├── components/
│   │   ├── Navbar.jsx
│   │   ├── Sidebar.jsx
│   │   └── Player.jsx
│   │
│   ├── context/
│   │
│   ├── App.jsx
│   ├── index.css
│   └── main.jsx
│
├── .gitignore
├── eslint.config.js
├── index.html
├── package.json
├── package-lock.json
├── README.md
└── vite.config.js
```

The exact file structure may change as the project is extended.

---

## Main Components

### Sidebar

The Sidebar provides the main navigation and library area.

It contains:
- Home
- Search
- Your Library
- Create Playlist
- Podcast discovery

The component uses Tailwind CSS responsive classes to control its visibility and layout on different screen sizes.

### Navbar

The Navbar provides the top-level controls for the main content area.

It includes:
- Back/forward controls
- Explore Premium
- Install App
- User profile
- Music category filters

### Player

The Player provides the music playback interface.

It displays:
- Song artwork
- Song name
- Song description
- Playback controls
- Shuffle
- Previous
- Play/pause
- Next
- Repeat
- Playback progress
- Current time
- Total duration

### Music Cards

Music and playlist cards are used to display:
- Artwork
- Song/playlist title
- Description
- Featured collections

---

## Audio Playback

The project uses local audio assets rather than a remote music streaming service.

The basic flow is:

```text
User selects a song
        ↓
Song data is selected
        ↓
Audio file is loaded
        ↓
Browser plays the audio
        ↓
Player UI updates
```

This keeps the project self-contained on the frontend.

---

## Tailwind CSS

Tailwind CSS is used extensively for the interface.

Examples of the utility classes used in the project include:

```text
flex
items-center
justify-between
gap-4
bg-black
text-white
rounded-full
w-[25%]
h-[10%]
hidden
lg:flex
md:block
```

This allows the UI to be constructed directly in JSX while keeping the styling responsive.

---

## Responsive Design

Responsive behavior is implemented using Tailwind breakpoints.

For example:

```jsx
<div className="hidden lg:flex">
```

hides an element on smaller screens and displays it on large screens.

Similarly:

```text
hidden md:block
```

can be used to display an element only from the medium breakpoint upward.

---

## Installation

### Prerequisites

Make sure you have:

- Node.js
- npm

installed on your system.

### Clone the project

```bash
git clone <your-repository-url>
```

### Enter the project directory

```bash
cd song-player
```

### Install dependencies

```bash
npm install
```

### Start the development server

```bash
npm run dev
```

Vite will provide a local development URL, normally:

```text
http://localhost:5173/
```

---

## Build for Production

To create a production build:

```bash
npm run build
```

To preview the production build locally:

```bash
npm run preview
```

---

## Current Limitations

This project is currently a frontend implementation.

It does not currently provide:

- User authentication
- Backend services
- Database storage
- Persistent user playlists
- Spotify account integration
- Spotify Web API integration
- Online music catalog
- Cloud music storage
- User-specific recommendations
- Real-time synchronization between devices

The songs, images, and other media used by the application are handled through project assets.

---

## Future Improvements

Possible future additions include:

### Backend
- User authentication
- Database integration
- Persistent playlists
- Liked songs
- Recently played songs
- User profiles

### Music Features
- Search functionality
- Dynamic song queues
- Volume control
- Seekable progress bar
- Improved shuffle logic
- Repeat modes
- Playlist creation and editing
- Favorite songs

### API Integration
A future version could connect to a suitable music service API to dynamically retrieve:
- Artists
- Albums
- Songs
- Playlists
- Search results

### UI/UX
- Mobile navigation drawer
- Animations and transitions
- Loading states
- Better accessibility
- Keyboard controls
- Improved mobile player
- More detailed song and artist pages

---

## Learning Outcomes

This project provides practical experience with:

- React component architecture
- JSX
- JavaScript
- Tailwind CSS
- Responsive web design
- Vite
- npm
- Local asset management
- Browser audio playback
- Component composition
- Frontend debugging
- Browser developer tools

---

## Project Status

**Status:** Frontend development / learning project

The current version focuses on the UI and client-side music playback experience.

---

## Credits and Attribution

This project is a Spotify-inspired educational project and is based on a tutorial/reference implementation.

Spotify is a trademark of Spotify AB. This project is not affiliated with, sponsored by, or endorsed by Spotify.

If you publish a substantially copied version of an existing tutorial/repository, retain appropriate attribution to the original creator and comply with the original repository's license and the licenses of any included assets.

---

## Author

Mayank Lohan

B.Tech - Electronics & Communication Engineering  
National Institute of Technology, Rourkela

