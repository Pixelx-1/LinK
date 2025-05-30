# Accessibility Hub

A web-based centralized directory and interactive platform for open-source assistive AI tools, designed to help people with disabilities discover and use AI-powered aids in an accessible interface.

## 🌟 Overview

The Accessibility Hub serves as a comprehensive platform that promotes digital inclusion by providing:

- **Tool Directory**: A searchable, categorized catalog of assistive AI tools
- **Interactive Demos**: In-app demonstrations of AI-powered accessibility tools
- **AI Assistant**: LLM-based chatbot for accessibility guidance
- **Accessibility Settings**: Built-in UI controls for personal preferences
- **Community Contributions**: User-driven tool submissions and feedback

With over 1 billion people worldwide living with disabilities (16% of the global population), this platform ensures compliance with WCAG and WAI-ARIA standards for broad impact and inclusive digital experiences.

## 🚀 Features

### Core Features
- **Searchable Tool Directory**: Find assistive tools by keywords, categories, or functionality
- **Category-Based Organization**: Tools organized by Visual, Auditory, Motor, and Cognitive assistance
- **Interactive Demos**: Try tools like image captioning, speech-to-text, and text simplification
- **AI Chatbot Assistant**: Get answers to accessibility questions using open-source LLMs
- **ASL Alphabet Learning**: Complete alphabet with hand gesture emojis and interactive learning modes
- **Accessibility Controls**: High-contrast mode, large text, reduced motion settings
- **User Contributions**: Submit new tools and provide feedback

### ASL Hand Sign Features
- **Real Photographs**: All 26 alphabet signs use actual photographs of ASL hand positions
- **Authentic Accuracy**: Professional-quality images showing exact finger placement and hand orientation
- **Educational Quality**: Real human hands demonstrating proper ASL alphabet signing techniques
- **Optimized Format**: Standardized 150x150 pixel images with clean backgrounds for clarity
- **Fast Loading**: Processed and optimized for quick display and smooth user experience
- **Learning Excellence**: Perfect visual references for serious ASL alphabet study

### Accessibility Features
- **WCAG 2.1 AA Compliance**: Meets accessibility guidelines
- **Keyboard Navigation**: Full functionality without mouse
- **Screen Reader Support**: Semantic HTML and ARIA labels
- **High Contrast Mode**: Enhanced visibility options
- **Focus Management**: Clear focus indicators and logical tab order
- **Skip Links**: Quick navigation for screen reader users

## 🛠️ Tech Stack

### Frontend
- **React 18** with TypeScript
- **Tailwind CSS** for styling with accessibility-focused design
- **React Router** for navigation
- **Heroicons** for accessible icons
- **Axios** for API communication

### Backend
- **Node.js** with Express and TypeScript
- **PostgreSQL** or **MongoDB** for data storage
- **CORS** and **Helmet** for security
- **Multer** for file uploads

### AI/ML Integration
- **Hugging Face Transformers** for open-source LLMs
- **Whisper ASR** for speech-to-text
- **BLIP/Vision Models** for image captioning
- **Tesseract OCR** for text extraction
- **Mozilla TTS** for text-to-speech

### Development Tools
- **ESLint** with jsx-a11y plugin for accessibility linting
- **axe-core** for automated accessibility testing
- **TypeScript** for type safety
- **Prettier** for code formatting

## 📁 Project Structure

```
accessibility-hub/
├── frontend/                 # React frontend application
│   ├── src/
│   │   ├── components/      # Reusable UI components
│   │   ├── pages/          # Page-level components
│   │   ├── styles/         # CSS and Tailwind configs
│   │   └── utils/          # Helper functions
│   ├── public/             # Static assets
│   └── package.json
├── backend/                 # Node.js backend API
│   ├── src/
│   │   ├── controllers/    # Business logic
│   │   ├── models/         # Database models
│   │   ├── routes/         # API routes
│   │   ├── services/       # AI model services
│   │   └── utils/          # Shared utilities
│   └── package.json
├── tests/                  # Test suites
├── .github/workflows/      # CI/CD pipelines
└── README.md
```

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ and npm
- PostgreSQL or MongoDB (optional for basic functionality)
- Git

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/accessibility-hub.git
   cd accessibility-hub
   ```

2. **Install frontend dependencies**
   ```bash
   cd frontend
   npm install
   ```

3. **Install backend dependencies**
   ```bash
   cd ../backend
   npm install
   ```

4. **Configure environment variables**
   ```bash
   # Copy example environment file
   cp .env.example .env
   # Edit .env with your configuration
   ```

5. **Start the development servers**

   **Frontend** (in one terminal):
   ```bash
   cd frontend
   npm start
   ```

   **Backend** (in another terminal):
   ```bash
   cd backend
   npm run dev
   ```

6. **Access the application**
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:5000
   - Health check: http://localhost:5000/health

## 🎯 Usage

### For Users
1. **Browse Tools**: Visit the homepage and explore tool categories
2. **Search**: Use the search bar to find specific assistive tools
3. **Try Demos**: Click on tools to access interactive demonstrations
4. **Ask AI**: Use the chatbot for accessibility guidance
5. **Customize**: Adjust accessibility settings in the header menu

### For Developers
1. **Add Tools**: Contribute new assistive tools via the submission form
2. **API Integration**: Use the REST API for tool data and AI services
3. **Extend Features**: Follow the component structure to add new functionality

## 🧪 Testing

### Accessibility Testing
```bash
# Run automated accessibility tests
npm run test:a11y

# Manual testing checklist:
# - Keyboard navigation (Tab, Enter, Space, Arrow keys)
# - Screen reader compatibility (NVDA, JAWS, VoiceOver)
# - Color contrast validation
# - Focus management
```

### Unit Testing
```bash
# Frontend tests
cd frontend && npm test

# Backend tests
cd backend && npm test
```

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

### Development Workflow
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes following our coding standards
4. Run accessibility tests (`npm run test:a11y`)
5. Commit your changes (`git commit -m 'Add amazing feature'`)
6. Push to the branch (`git push origin feature/amazing-feature`)
7. Open a Pull Request

### Accessibility Guidelines
- Follow WCAG 2.1 AA standards
- Use semantic HTML elements
- Provide alt text for images
- Ensure keyboard accessibility
- Test with screen readers
- Maintain color contrast ratios

## 📊 API Documentation

### Endpoints

#### Tools
- `GET /api/tools` - List all tools
- `GET /api/tools/:id` - Get tool details
- `POST /api/tools` - Submit new tool (authenticated)

#### AI Services
- `POST /api/chat` - Chat with AI assistant
- `POST /api/alt-text` - Generate image alt text
- `POST /api/transcribe` - Speech-to-text transcription
- `POST /api/simplify` - Text simplification

#### Health
- `GET /health` - API health check

## 🔧 Configuration

### Environment Variables
```bash
# Server
PORT=5000
NODE_ENV=development
FRONTEND_URL=http://localhost:3000

# Database
DATABASE_URL=postgresql://localhost:5432/accessibility_hub
MONGODB_URI=mongodb://localhost:27017/accessibility_hub

# AI Services
HUGGINGFACE_API_KEY=your_api_key_here

# Security
JWT_SECRET=your_jwt_secret
```

## 📈 Roadmap

- [ ] **Phase 1**: Core platform with basic tool directory
- [ ] **Phase 2**: AI-powered demos (image captioning, speech-to-text)
- [ ] **Phase 3**: Advanced chatbot with accessibility expertise
- [ ] **Phase 4**: Community features and user accounts
- [ ] **Phase 5**: Mobile app and offline capabilities
- [ ] **Phase 6**: Integration with popular accessibility tools

## 🏆 Accessibility Compliance

This project aims for **WCAG 2.1 AA compliance** and includes:

- ✅ Semantic HTML structure
- ✅ ARIA labels and roles
- ✅ Keyboard navigation support
- ✅ Screen reader compatibility
- ✅ High contrast mode
- ✅ Focus management
- ✅ Alternative text for images
- ✅ Accessible forms and error handling

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Web Content Accessibility Guidelines (WCAG)](https://www.w3.org/WAI/WCAG21/quickref/)
- [WAI-ARIA Authoring Practices](https://www.w3.org/WAI/ARIA/apg/)
- [Hugging Face](https://huggingface.co/) for open-source AI models
- [WebAIM](https://webaim.org/) for accessibility resources
- The global accessibility community for guidance and feedback

## 📞 Support

- **Documentation**: [Wiki](https://github.com/your-username/accessibility-hub/wiki)
- **Issues**: [GitHub Issues](https://github.com/your-username/accessibility-hub/issues)
- **Discussions**: [GitHub Discussions](https://github.com/your-username/accessibility-hub/discussions)
- **Email**: contact@accessibilityhub.org

---

**Making technology accessible for everyone** 🌍♿ 