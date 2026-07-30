# Sociocultural Project Development Environment

> An open-source, offline-first, accessible workflow for bottom-up, participatory, and locally-led sociocultural projects.

## 🌟 Ethical Principles

This project is built on the following ethical foundations:

- ✅ **Open Source**: All code is freely available and modifiable
- ✅ **Accessible**: Designed for users with varying abilities and language skills
- ✅ **Easy to Use**: Intuitive interface with minimal learning curve
- ✅ **Offline-First**: Fully functional without internet connection
- ✅ **Data Protection**: Local data storage with privacy by design
- ✅ **Data Light**: Minimal resource usage for ecological sustainability

## 📋 Overview

This environment supports sociocultural project development through **7 distinct phases**:

1. **Setup** - Professionals define project context
2. **Pre-Project** - Community data collection (notes, photos, observations)
3. **Topic Selection** - Cluster data and select focus area
4. **Situation Analysis** - Comprehensive analysis using participatory methods
5. **Conceptualisation** - Develop Theory of Change, stakeholder maps, intervention plans
6. **Implementation** - Execute with monitoring and evaluation tools
7. **Evaluation** - Assess outcomes and impact

## 🚀 Quick Start

### For Users

1. **Download/Install** the application (options below)
2. **Create a new project** with your theme/context
3. **Invite team members** (optional, for multi-user setups)
4. **Start collecting data** in the Pre-Project phase
5. **Follow the workflow** through each phase

### For Developers

1. Clone this repository:
   ```bash
   git clone https://github.com/johanneskueng/community_based_project_dev.git
   cd community_based_project_dev
   ```

2. Read the documentation:
   - [Workflow Design](docs/WORKFLOW_DESIGN.md) - Detailed workflow specification
   - [Visual Workflow](docs/WORKFLOW_VISUAL.md) - Diagrams and flow charts
   - [Implementation Guide](docs/IMPLEMENTATION_GUIDE.md) - Technical implementation details

3. Choose your development path:
   - [PWA (Recommended)](docs/IMPLEMENTATION_GUIDE.md#option-1-web-based-progressive-web-app---pwa)
   - [Desktop Application](docs/IMPLEMENTATION_GUIDE.md#option-2-desktop-application)
   - [Mobile Application](docs/IMPLEMENTATION_GUIDE.md#option-3-mobile-application)

## 📦 Installation Options

### Option 1: Progressive Web App (PWA)
- **No installation required** - Use directly in browser
- **Install to home screen** - Browser will prompt to "Add to Home Screen"
- **Works offline** - After first load, works without internet

### Option 2: Desktop Application
- **Windows**: Download `.exe` installer
- **macOS**: Download `.dmg` file
- **Linux**: Download `.AppImage` or `.deb`/`.rpm` packages

### Option 3: Mobile Application
- **Android**: Download from Google Play Store
- **iOS**: Download from Apple App Store

### Option 4: Offline Distribution
- **USB Drive**: Copy files to USB for distribution
- **Local Server**: Host on local network server
- **CD/DVD**: For areas with very limited connectivity

## 🎯 Features

### Core Features (MVP)
- ✅ Project setup and configuration
- ✅ Data collection (text notes, photos)
- ✅ Data clustering and topic selection
- ✅ Basic situation analysis
- ✅ Offline functionality
- ✅ Multiple language support
- ✅ Accessibility features
- ✅ Data export/import

### Advanced Features (Roadmap)
- 🔄 Theory of Change builder
- 🔄 Stakeholder mapping tools
- 🔄 Intervention planning
- 🔄 Budget calculation
- 🔄 Monitoring and evaluation framework
- 🔄 Multi-device synchronization
- 🔄 Advanced reporting

## 📂 Project Structure

```
community_based_project_dev/
├── docs/                          # Documentation
│   ├── WORKFLOW_DESIGN.md         # Detailed workflow
│   ├── WORKFLOW_VISUAL.md         # Visual representations
│   └── IMPLEMENTATION_GUIDE.md    # Technical guide
│
├── src/                           # Source code (after implementation)
│   ├── frontend/                   # Frontend application
│   ├── backend/                    # Backend code (optional)
│   └── shared/                     # Shared utilities
│
├── data/                          # Local data (created at runtime)
│   ├── projects/
│   ├── users/
│   └── backups/
│
├── tests/                         # Tests
│   ├── unit/
│   ├── integration/
│   └── e2e/
│
├── scripts/                       # Utility scripts
│
├── .gitignore
├── LICENSE
└── README.md
```

## 🛠️ Development Setup

### Prerequisites
- Node.js 18+ (for PWA/desktop)
- npm or yarn
- Git

### Installation
```bash
# Clone the repository
git clone https://github.com/johanneskueng/community_based_project_dev.git
cd community_based_project_dev

# Install dependencies (after implementation)
npm install

# Start development server
npm run dev
```

### Building
```bash
# Build for production
npm run build

# Build for specific platforms
npm run build:pwa      # Progressive Web App
npm run build:desktop  # Desktop application
npm run build:mobile   # Mobile application
```

## 🤝 Contributing

We welcome contributions! Please read our [Contributing Guide](CONTRIBUTING.md) for details on:

- How to report bugs
- How to suggest features
- How to contribute code
- Coding standards
- Testing requirements

## 📄 Documentation

- [Workflow Design](docs/WORKFLOW_DESIGN.md) - Complete workflow specification
- [Visual Workflow](docs/WORKFLOW_VISUAL.md) - Diagrams and flow charts
- [Implementation Guide](docs/IMPLEMENTATION_GUIDE.md) - Technical implementation
- [User Guides](docs/USER_GUIDES/) - Step-by-step user instructions
- [Technical Docs](docs/TECHNICAL/) - API reference, architecture, etc.

## 🌍 Community

- **Issues**: [GitHub Issues](https://github.com/johanneskueng/community_based_project_dev/issues)
- **Discussions**: [GitHub Discussions](https://github.com/johanneskueng/community_based_project_dev/discussions)
- **Contributing**: [Contributing Guide](CONTRIBUTING.md)

## 📜 License

This project is licensed under the [MIT License](LICENSE) - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by participatory development methodologies
- Built with open-source technologies
- Designed for community empowerment

---

## 📞 Support

For support, please:

1. Check the [documentation](docs/)
2. Search [existing issues](https://github.com/johanneskueng/community_based_project_dev/issues)
3. Open a [new issue](https://github.com/johanneskueng/community_based_project_dev/issues/new)

---

*Project Status: 🏗️ Workflow Design Complete | Implementation Pending*

*Last Updated: 2024*
