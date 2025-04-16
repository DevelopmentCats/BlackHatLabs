# BHLabs (Black Hat Labs)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

BHLabs is a multiplayer and single-player browser-based hacking simulation game designed to realistically emulate and teach cybersecurity concepts. The game offers both PVE (Player vs. Environment) and PVP (Player vs. Player) scenarios, providing an engaging platform for learning ethical hacking skills.

## Features

- **Terminal Emulation**: Realistic command-line interface for executing hacking commands
- **Network Simulation**: Virtual network topology with interconnected systems
- **Hacking Tools**: Collection of simulated reconnaissance, exploitation, and post-exploitation tools
- **Challenge System**: Progressive difficulty levels with multiple solution paths
- **Skill Progression**: Specialized skill paths and unlockable abilities
- **Educational Content**: Integrated cybersecurity learning materials
- **Multiplayer**: PvP and cooperative PvE gameplay modes
- **Self-Hostable**: Easy deployment on your own infrastructure

## Getting Started

### Prerequisites

- Node.js (v16.x or later)
- npm or yarn package manager
- Git for version control
- Docker for containerization (optional for development, required for deployment)

### Development Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/bhlabs.git
   cd bhlabs
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run the development server:
   ```bash
   # Start the client development server
   cd client
   npm run dev

   # In a separate terminal, start the server
   cd server
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:3000`

### Docker Setup (for deployment)

1. Build and start the containers:
   ```bash
   docker-compose up -d
   ```

2. Access the application at `http://localhost`

## Project Structure

```
bhlabs/
├── client/                     # Frontend code
│   ├── public/                 # Static assets
│   │   ├── src/                    # Source code
│   │   │   ├── components/         # React components
│   │   │   ├── game/               # Game-specific code
│   │   │   │   ├── core/           # Core game mechanics
│   │   │   │   ├── ui/             # Game UI components
│   │   │   │   ├── entities/       # Game entities
│   │   │   │   └── systems/        # Game systems
│   │   │   ├── services/           # API and WebSocket services
│   │   │   ├── utils/              # Utility functions
│   │   │   └── assets/             # Game assets
├── server/                     # Backend code
│   ├── src/                    # Source code
│   │   ├── api/                # REST API endpoints
│   │   ├── game/               # Game logic
│   │   ├── websocket/          # WebSocket handlers
│   │   ├── database/           # Database models and migrations
│   │   ├── services/           # Business logic services
│   │   └── utils/              # Utility functions
├── shared/                     # Shared code between client and server
│   ├── constants/              # Shared constants
│   ├── types/                  # TypeScript type definitions
│   └── utils/                  # Shared utility functions
├── docs/                       # Documentation
├── scripts/                    # Build and deployment scripts
└── docker/                     # Docker configuration
```

## Technology Stack

- **Frontend**: React, TypeScript, Phaser/Three.js
- **Backend**: Node.js, Express, TypeScript
- **Database**: PostgreSQL, Redis
- **Testing**: Jest, Cypress
- **DevOps**: Docker, GitHub Actions
- **Communication**: WebSockets (Socket.io)

## Contributing

We welcome contributions to BHLabs! Please see our [Contributing Guide](CONTRIBUTING.md) for more details.

## Educational Focus

BHLabs is designed with education in mind:

- **Learning Modules**: Structured tutorials on cybersecurity concepts
- **Real-World Relevance**: Scenarios based on actual vulnerabilities
- **Ethical Hacking**: Focus on responsible disclosure and ethical considerations
- **Progressive Learning**: From basic concepts to advanced techniques

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Inspired by platforms like Hack The Box, TryHackMe, and other cybersecurity training tools
- Special thanks to all contributors and the cybersecurity education community

## Contact

For questions, suggestions, or issues, please open an issue on the GitHub repository. 