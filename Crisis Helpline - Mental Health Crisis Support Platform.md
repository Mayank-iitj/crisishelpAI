# Crisis Helpline - Mental Health Crisis Support Platform

<div align="center">
  <img src="assets/images/logo.png" alt="MindCare Logo" width="200"/>
  
  [![Live Demo](https://img.shields.io/badge/Live%20Demo-Visit%20Site-blue?style=for-the-badge)](https://crisishelpline.netlify.app/)
  [![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
  [![Contributions Welcome](https://img.shields.io/badge/Contributions-Welcome-orange?style=for-the-badge)](CONTRIBUTING.md)
  
  **आप अकेले नहीं हैं - You Are Not Alone**
  
  *India's Most Trusted Mental Health Platform*
</div>

---

## 🌟 Overview

Crisis Helpline is a comprehensive mental health crisis support platform designed specifically for India, providing 24/7 AI-powered mental health support, community resources, culturally-aware assistance, and professional help when needed most. The platform connects users with local resources, verified emergency services across 28 states, and a supportive community of peers who understand the unique challenges faced in the Indian context.

<div align="center">
  <img src="assets/images/hero-banner.png" alt="Mental Health Crisis Support" width="100%"/>
</div>

### 🎯 Mission Statement

Our mission is to break the stigma surrounding mental health in India while providing immediate, accessible, and culturally sensitive support to individuals experiencing mental health crises. We believe that no one should face their darkest moments alone, and through technology, community, and compassion, we can create a safety net that saves lives.




## ✨ Key Features

<div align="center">
  <img src="assets/images/features-overview.png" alt="Platform Features Overview" width="100%"/>
</div>

### 🤖 24/7 AI-Powered Chat Support
Our advanced AI chatbot provides immediate emotional support and crisis intervention, trained specifically on mental health protocols and Indian cultural contexts. The system can:
- Detect crisis situations and escalate appropriately
- Provide coping strategies and breathing exercises
- Offer multilingual support in major Indian languages
- Connect users to human counselors when needed

### 📞 Emergency Helplines Integration
Direct access to verified emergency mental health services across all 28 Indian states, including:
- **National Suicide Prevention Lifeline**: 112
- **KIRAN Mental Health Helpline**: 1800-599-0019
- State-specific crisis intervention numbers
- 24/7 availability with multilingual support

### 📊 Mood Tracking & Analytics
Comprehensive mood tracking system that helps users:
- Monitor emotional patterns over time
- Identify triggers and warning signs
- Share progress with healthcare providers
- Receive personalized insights and recommendations

### 🎵 Therapeutic Music & Meditation
Curated collection of calming music, guided meditations, and breathing exercises designed to:
- Reduce anxiety and stress levels
- Promote relaxation and mindfulness
- Support sleep and recovery
- Provide immediate coping tools during crisis moments

### 👥 Community Support Network
Safe, moderated community spaces where users can:
- Share experiences and stories anonymously
- Connect with peers facing similar challenges
- Access peer support groups
- Participate in guided discussions with mental health professionals

<div align="center">
  <img src="assets/images/community-support.png" alt="Community Support Network" width="100%"/>
</div>

### 📚 Resource Library
Extensive collection of mental health resources including:
- Educational articles on mental health conditions
- Self-help guides and coping strategies
- Information about local mental health services
- Crisis intervention protocols and safety planning tools

### 🏥 Crisis Intervention Protocol
Immediate crisis response system featuring:
- Real-time risk assessment algorithms
- Automatic escalation to emergency services
- GPS-based local resource recommendations
- Follow-up care coordination


## 🛠️ Technology Stack

### Frontend Technologies
- **HTML5/CSS3**: Modern semantic markup and responsive styling
- **JavaScript (ES6+)**: Interactive functionality and dynamic content
- **Tailwind CSS**: Utility-first CSS framework for rapid UI development
- **Lucide Icons**: Beautiful, customizable icon library
- **Progressive Web App (PWA)**: Offline functionality and mobile app-like experience

### Backend & Infrastructure
- **Node.js**: Server-side JavaScript runtime
- **Express.js**: Web application framework
- **WebSocket**: Real-time communication for chat functionality
- **RESTful APIs**: Standardized data exchange protocols

### Database & Storage
- **MongoDB**: NoSQL database for user data and chat logs
- **Redis**: In-memory caching for session management
- **Cloud Storage**: Secure file storage for user uploads and resources

### AI & Machine Learning
- **Natural Language Processing**: Crisis detection and sentiment analysis
- **OpenAI GPT Integration**: Advanced conversational AI capabilities
- **TensorFlow.js**: Client-side machine learning for mood analysis

### Security & Privacy
- **HTTPS/TLS 1.3**: End-to-end encryption for all communications
- **JWT Authentication**: Secure user session management
- **GDPR Compliance**: Privacy-first data handling practices
- **HIPAA-Level Security**: Healthcare-grade data protection

## 🏗️ System Architecture

<div align="center">
  <img src="assets/images/architecture-diagram.png" alt="System Architecture Diagram" width="100%"/>
</div>

The Crisis Helpline platform follows a modern, scalable microservices architecture designed for high availability and security. The system is built with the following core components:

### Frontend Layer
The user interface is built as a responsive web application that adapts seamlessly across desktop, tablet, and mobile devices. The frontend communicates with backend services through secure REST APIs and maintains real-time connections via WebSocket for chat functionality.

### API Gateway
A centralized API gateway handles all incoming requests, providing authentication, rate limiting, and request routing to appropriate microservices. This layer ensures security and scalability while maintaining a clean separation of concerns.

### Core Services
- **User Authentication Service**: Manages user registration, login, and session handling
- **Chat Service**: Handles real-time messaging and AI integration
- **Crisis Detection Service**: Monitors conversations for crisis indicators
- **Resource Management Service**: Manages educational content and emergency contacts
- **Analytics Service**: Processes mood tracking data and generates insights

### Data Layer
The platform uses a hybrid database approach with MongoDB for user data and chat logs, Redis for session caching, and specialized storage for AI model data and analytics.

## 📱 Responsive Design

<div align="center">
  <img src="assets/images/mobile-responsive.png" alt="Responsive Design Showcase" width="100%"/>
</div>

The platform is designed with a mobile-first approach, ensuring optimal user experience across all devices. Key responsive features include:

- **Adaptive Layout**: Fluid grid system that adjusts to any screen size
- **Touch-Friendly Interface**: Large tap targets and gesture support
- **Optimized Performance**: Fast loading times on mobile networks
- **Offline Functionality**: Core features available without internet connection
- **Accessibility**: WCAG 2.1 AA compliance for users with disabilities


## 🚀 Quick Start

### Prerequisites
Before setting up the Crisis Helpline platform, ensure you have the following installed:

- **Node.js** (version 16.0 or higher)
- **npm** or **yarn** package manager
- **Git** for version control
- **MongoDB** (local installation or cloud instance)
- **Redis** (for session management)

### Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/username/crisis-helpline.git
   cd crisis-helpline
   ```

2. **Install Dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Environment Configuration**
   Create a `.env` file in the root directory:
   ```env
   # Database Configuration
   MONGODB_URI=mongodb://localhost:27017/crisis-helpline
   REDIS_URL=redis://localhost:6379
   
   # API Keys
   OPENAI_API_KEY=your_openai_api_key_here
   TWILIO_ACCOUNT_SID=your_twilio_sid
   TWILIO_AUTH_TOKEN=your_twilio_token
   
   # Security
   JWT_SECRET=your_jwt_secret_key
   SESSION_SECRET=your_session_secret
   
   # External Services
   GOOGLE_ANALYTICS_ID=your_analytics_id
   SENTRY_DSN=your_sentry_dsn
   ```

4. **Database Setup**
   ```bash
   # Start MongoDB service
   sudo systemctl start mongod
   
   # Start Redis service
   sudo systemctl start redis
   
   # Run database migrations
   npm run migrate
   ```

5. **Start Development Server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

6. **Access the Application**
   Open your browser and navigate to `http://localhost:3000`

### Production Deployment

For production deployment, follow these additional steps:

1. **Build the Application**
   ```bash
   npm run build
   ```

2. **Configure Production Environment**
   Update your `.env` file with production values:
   ```env
   NODE_ENV=production
   PORT=80
   MONGODB_URI=your_production_mongodb_uri
   REDIS_URL=your_production_redis_url
   ```

3. **Deploy to Hosting Platform**
   
   **Netlify Deployment:**
   ```bash
   # Build command
   npm run build
   
   # Publish directory
   dist/
   ```
   
   **Vercel Deployment:**
   ```bash
   vercel --prod
   ```
   
   **Docker Deployment:**
   ```bash
   docker build -t crisis-helpline .
   docker run -p 80:3000 crisis-helpline
   ```

## 💻 Usage Guide

### For Users

#### Getting Started
1. **Visit the Platform**: Navigate to [crisishelpline.netlify.app](https://crisishelpline.netlify.app/)
2. **Create Account**: Register with email or use anonymous access for immediate support
3. **Complete Safety Assessment**: Brief questionnaire to personalize your experience
4. **Access Support**: Choose from chat support, emergency contacts, or community resources

#### Using Chat Support
1. Click "Start Chat Now" on the homepage
2. Describe your situation in your own words
3. The AI will provide immediate support and coping strategies
4. Request human counselor if needed
5. Access follow-up resources and safety planning tools

#### Emergency Situations
1. Click "Crisis Support" for immediate help
2. Access emergency hotlines with one-click calling
3. Share location for local emergency services
4. Use safety planning tools and crisis intervention protocols

#### Community Features
1. Join anonymous support groups
2. Share experiences and read others' stories
3. Participate in guided discussions
4. Access peer mentorship programs

### For Developers

#### Project Structure
```
crisis-helpline/
├── src/
│   ├── components/          # Reusable UI components
│   ├── pages/              # Application pages
│   ├── services/           # API and external service integrations
│   ├── utils/              # Utility functions and helpers
│   └── styles/             # CSS and styling files
├── public/
│   ├── assets/             # Static assets (images, icons)
│   └── index.html          # Main HTML template
├── docs/                   # Documentation files
├── tests/                  # Test suites
└── config/                 # Configuration files
```

#### Development Workflow
1. **Create Feature Branch**: `git checkout -b feature/new-feature`
2. **Make Changes**: Implement your feature with tests
3. **Run Tests**: `npm test` to ensure code quality
4. **Commit Changes**: Use conventional commit messages
5. **Push and Create PR**: Submit for code review
6. **Deploy**: Automatic deployment after merge to main

#### API Integration
```javascript
// Example: Starting a chat session
const startChat = async (urgencyLevel) => {
  const response = await fetch('/api/chat/start', {
    method: 'POST',
    headers: {
      'Content-Type': 'application/json',
      'Authorization': `Bearer ${token}`
    },
    body: JSON.stringify({ urgencyLevel })
  });
  
  return response.json();
};

// Example: Sending a message
const sendMessage = async (sessionId, message) => {
  const response = await fetch('/api/chat/message', {
    method: 'POST',
    headers: {
      'Content-Type': 'application/json',
      'Authorization': `Bearer ${token}`
    },
    body: JSON.stringify({ sessionId, message })
  });
  
  return response.json();
};
```


## 🤝 Contributing

We welcome contributions from developers, mental health professionals, and community members who want to help improve mental health support accessibility. Please read our [Contributing Guidelines](CONTRIBUTING.md) for detailed information.

### Ways to Contribute

#### For Developers
- **Bug Fixes**: Help identify and fix issues in the codebase
- **Feature Development**: Implement new features and improvements
- **Performance Optimization**: Enhance application speed and efficiency
- **Security Enhancements**: Strengthen platform security measures
- **Documentation**: Improve code documentation and user guides

#### For Mental Health Professionals
- **Content Review**: Validate mental health information and resources
- **Crisis Protocol Development**: Help design effective intervention strategies
- **Training Data**: Contribute to AI training with appropriate clinical guidance
- **User Experience Testing**: Provide feedback on platform usability

#### For Community Members
- **User Testing**: Test new features and provide feedback
- **Translation**: Help translate content into regional Indian languages
- **Resource Curation**: Suggest valuable mental health resources
- **Advocacy**: Help spread awareness about mental health support

### Development Guidelines

#### Code Standards
- Follow ESLint configuration for JavaScript code style
- Use Prettier for consistent code formatting
- Write comprehensive unit tests for new features
- Maintain minimum 80% code coverage
- Document all public APIs and complex functions

#### Commit Message Format
```
type(scope): description

[optional body]

[optional footer]
```

Examples:
```
feat(chat): add crisis detection algorithm
fix(auth): resolve session timeout issue
docs(readme): update installation instructions
```

#### Pull Request Process
1. Fork the repository and create a feature branch
2. Make your changes with appropriate tests
3. Update documentation as needed
4. Ensure all tests pass and code coverage is maintained
5. Submit pull request with clear description of changes
6. Respond to code review feedback promptly

## 🧪 Testing

### Test Suite Overview
The platform includes comprehensive testing to ensure reliability and safety:

#### Unit Tests
```bash
# Run all unit tests
npm test

# Run tests with coverage
npm run test:coverage

# Run tests in watch mode
npm run test:watch
```

#### Integration Tests
```bash
# Run integration tests
npm run test:integration

# Test API endpoints
npm run test:api

# Test database operations
npm run test:db
```

#### End-to-End Tests
```bash
# Run E2E tests
npm run test:e2e

# Run E2E tests in headless mode
npm run test:e2e:headless

# Test critical user journeys
npm run test:critical-path
```

#### Performance Tests
```bash
# Run performance benchmarks
npm run test:performance

# Load testing
npm run test:load

# Memory leak detection
npm run test:memory
```

### Testing Guidelines
- Write tests for all new features and bug fixes
- Maintain minimum 80% code coverage
- Test critical user journeys thoroughly
- Include accessibility testing in test suites
- Perform security testing for sensitive operations

## 📊 Analytics & Monitoring

### User Analytics
The platform includes privacy-respecting analytics to improve user experience:

- **Usage Patterns**: Understanding how users interact with features
- **Crisis Intervention Effectiveness**: Measuring support success rates
- **Performance Metrics**: Monitoring application speed and reliability
- **User Satisfaction**: Collecting feedback through surveys and ratings

### System Monitoring
- **Uptime Monitoring**: 99.9% availability target
- **Error Tracking**: Real-time error detection and alerting
- **Performance Monitoring**: Response time and resource usage tracking
- **Security Monitoring**: Threat detection and prevention

### Privacy Protection
All analytics are collected with strict privacy protections:
- No personally identifiable information is stored
- Data is anonymized and aggregated
- Users can opt-out of analytics collection
- GDPR and Indian data protection law compliance

## 🔒 Security & Privacy

### Data Protection
- **End-to-End Encryption**: All communications are encrypted in transit
- **Data Minimization**: Only necessary data is collected and stored
- **Secure Storage**: Healthcare-grade security for sensitive information
- **Regular Audits**: Quarterly security assessments and penetration testing

### Privacy Measures
- **Anonymous Access**: Users can access support without creating accounts
- **Data Retention**: Automatic deletion of chat logs after 30 days
- **User Control**: Complete control over personal data and deletion
- **Transparency**: Clear privacy policy and data usage explanations

### Compliance
- **HIPAA Compliance**: Healthcare data protection standards
- **GDPR Compliance**: European data protection regulations
- **Indian IT Act**: Compliance with Indian data protection laws
- **SOC 2 Type II**: Security and availability certification

## 🌍 Localization & Accessibility

### Language Support
The platform supports multiple Indian languages:
- **Hindi**: हिंदी भाषा समर्थन
- **English**: Primary language for interface
- **Bengali**: বাংলা ভাষার সহায়তা
- **Tamil**: தமிழ் மொழி ஆதரவு
- **Telugu**: తెలుగు భాష మద్దతు
- **Marathi**: मराठी भाषा समर्थन

### Accessibility Features
- **Screen Reader Support**: Compatible with NVDA, JAWS, and VoiceOver
- **Keyboard Navigation**: Full functionality without mouse
- **High Contrast Mode**: Enhanced visibility for users with visual impairments
- **Text Scaling**: Support for up to 200% text enlargement
- **Voice Commands**: Speech-to-text input for hands-free operation

### Cultural Sensitivity
- **Regional Customization**: Content adapted for different Indian regions
- **Cultural Context**: Mental health support considering Indian cultural norms
- **Family Involvement**: Options for family-inclusive support approaches
- **Religious Considerations**: Respectful integration of spiritual coping methods

## 📈 Roadmap & Future Features

### Short-term Goals (3-6 months)
- **Mobile App Development**: Native iOS and Android applications
- **Expanded Language Support**: Additional regional Indian languages
- **Telehealth Integration**: Video calling with licensed therapists
- **Enhanced AI Capabilities**: Improved crisis detection and response

### Medium-term Goals (6-12 months)
- **Wearable Device Integration**: Mood tracking through smartwatches
- **Family Support Features**: Resources and tools for family members
- **Professional Dashboard**: Tools for mental health professionals
- **Research Platform**: Anonymous data contribution for mental health research

### Long-term Vision (1-2 years)
- **International Expansion**: Adaptation for other countries and cultures
- **AI Therapy Sessions**: Advanced AI-powered therapeutic interventions
- **Predictive Analytics**: Early warning systems for mental health crises
- **Integration with Healthcare Systems**: Seamless connection with hospitals and clinics

## 📞 Emergency Resources

### National Helplines
- **Emergency Services**: 112 (National Emergency Number)
- **KIRAN Mental Health Helpline**: 1800-599-0019
- **Vandrevala Foundation**: 1860-2662-345
- **iCall**: 9152987821

### State-Specific Resources
The platform maintains an updated database of mental health resources across all 28 Indian states, including:
- Local crisis intervention centers
- Government mental health facilities
- NGO support services
- Community mental health programs

### International Resources
- **International Association for Suicide Prevention**: [https://www.iasp.info/resources/Crisis_Centres/](https://www.iasp.info/resources/Crisis_Centres/)
- **Crisis Text Line**: Text HOME to 741741 (US)
- **Samaritans**: 116 123 (UK)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

### Contributors
- **Mayank Sharma**: Project Creator and Lead Developer
- **Mental Health Professionals**: Clinical guidance and content validation
- **Community Contributors**: Feature development and testing
- **Translators**: Localization and cultural adaptation

### Organizations
- **KIRAN Mental Health Helpline**: Partnership for emergency services
- **Indian Psychiatric Society**: Clinical guidance and best practices
- **National Institute of Mental Health and Neurosciences (NIMHANS)**: Research collaboration
- **Vandrevala Foundation**: Resource sharing and support

### Technology Partners
- **OpenAI**: AI and natural language processing capabilities
- **Netlify**: Hosting and deployment infrastructure
- **MongoDB**: Database services and support
- **Twilio**: Communication services integration

## 📞 Support & Contact

### Technical Support
- **GitHub Issues**: [Report bugs and request features](https://github.com/username/crisis-helpline/issues)
- **Email**: support@crisishelpline.com
- **Documentation**: [Comprehensive guides and API documentation](docs/)

### Mental Health Support
- **Platform**: [crisishelpline.netlify.app](https://crisishelpline.netlify.app/)
- **24/7 Chat Support**: Available on the platform
- **Emergency**: Call 112 or 1800-599-0019

### Community
- **Discord**: Join our developer and community discussions
- **Twitter**: [@CrisisHelplineIN](https://twitter.com/CrisisHelplineIN)
- **LinkedIn**: [Crisis Helpline Community](https://linkedin.com/company/crisis-helpline)

---

<div align="center">
  <p><strong>Remember: You are not alone. Help is always available.</strong></p>
  <p><em>आप अकेले नहीं हैं। सहायता हमेशा उपलब्ध है।</em></p>
  
  [![Made with ❤️ in India](https://img.shields.io/badge/Made%20with%20❤️%20in-India-orange?style=for-the-badge)](https://crisishelpline.netlify.app/)
</div>

