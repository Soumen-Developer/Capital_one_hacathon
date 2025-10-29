# 🌾 FarmMate AI – Intelligent Agricultural Companion

**FarmMate AI** is an advanced agentic AI application designed to revolutionize farming support with intelligent, localized, and real-time agricultural guidance. From weather-based planning to comprehensive crop management and market insights — FarmMate AI delivers smart, multilingual, and farmer-friendly solutions for India's diverse agricultural community.

---

## 🧠 Why FarmMate AI?

In a country as vast and diverse as India, farmers often face:
- **Unpredictable weather patterns** affecting crop decisions
- **Lack of region-specific guidance** for optimal farming
- **Fragmented information systems** across multiple sources
- **Language barriers** preventing access to modern technology
- **Limited real-time market data** for informed selling decisions

**FarmMate AI** bridges these gaps using cutting-edge Agentic AI, multimodal inputs, and comprehensive real-time data integrations.

---

## 🚀 Key Features

### 🌤️ **Weather-Aware Planning**
- Real-time weather data integration
- AI recommendations based on 7-day forecasts
- Risk assessment for weather-sensitive operations

### 🧠 **Agentic Decision Support**
- Multi-agent AI system with specialized roles
- Proactive recommendations for each crop lifecycle stage
- Goal-driven decision support with confidence scoring

### 🗣️ **Multilingual Support**
- **Supported Languages**: Hindi, English, Punjabi, Gujarati, Marathi
- Voice and text input capabilities
- Culturally relevant responses

### 🧑‍🌾 **Farmer-Centric Design**
- Intuitive interface designed for low-tech users
- Step-by-step guidance with visual indicators
- Mobile-first responsive design

### 🛰️ **Comprehensive Data Integration**
- Satellite imagery analysis (planned)
- Real-time mandi price integration
- Soil health monitoring and recommendations
- Government scheme eligibility checking

### 🧩 **Modern Architecture**
- Microservices architecture with Docker
- WebSocket real-time communication
- RESTful APIs for integration
- Scalable cloud deployment

---

## 🏗️ Tech Stack

| Component | Technology | Purpose |
|-----------|------------|---------|
| 🌐 **Frontend** | React.js + Flutter | Web & Mobile interfaces |
| 🧠 **AI Engine** | Google Gemini + LangChain | Intelligent decision support |
| 🔙 **Backend** | Node.js + Express | API gateway & routing |
| 🐍 **AI Service** | Python + FastAPI | AI agents & processing |
| 🐳 **Containerization** | Docker + Docker Compose | Service orchestration |
| 🌩️ **Data Sources** | Weather APIs, Market APIs | Real-time data feeds |
| 💾 **Vector DB** | ChromaDB | Contextual memory storage |
| 🔌 **Communication** | WebSocket + Socket.IO | Real-time updates |

---

## 📦 Project Architecture

```
🌾 FarmMate-AI/
├── 📄 README.md                           # Main documentation
├── 📄 FLUTTER_INTEGRATION_GUIDE.md        # Flutter app integration
├── 📄 docker-compose.yml                  # Multi-service orchestration
├── 📄 DOCKER_DEPLOYMENT.md                # Deployment guide
│
├── 📁 scripts/                            # Startup utilities
│   ├── start-farmmate.ps1                # Windows startup
│   ├── start-farmmate.sh                 # Linux/Mac startup
│   ├── farmmate-ultra-simple.ps1         # Simple local dev
│   └── start-farmmate-simple-working.ps1  # Development mode
│
├── 📁 backend/                            # Express.js Gateway
│   ├── 📄 Dockerfile                     # Backend container
│   ├── 📄 package.json                   # Dependencies & scripts
│   ├── � README.md                      # Backend documentation
│   ├── 📁 src/
│   │   ├── index.js                      # Express server
│   │   ├── 📁 config/
│   │   │   └── languageConfig.js         # Multilingual support
│   │   ├── 📁 controller/
│   │   │   ├── healthController.js       # Health checks
│   │   │   └── wellcome.js               # Welcome endpoints
│   │   ├── 📁 router/
│   │   │   └── router.js                 # API routing
│   │   └── 📁 services/
│   │       └── socketService.js          # WebSocket handling
│   └── 📁 tests/                         # Comprehensive test suite
│       ├── run-all-tests.js              # Test orchestrator
│       ├── test-communication.js         # Basic connectivity
│       ├── test-direct-ai.js             # AI integration
│       ├── test-farm-query.js            # Single queries
│       └── test-comprehensive-farm.js    # Full workflow
│
├── 📁 agent-python/                      # AI Processing Engine
│   ├── 📄 Dockerfile                     # AI container
│   ├── 📄 requirement.txt                # Python dependencies
│   ├── 📄 README.md                      # AI documentation
│   ├── 📁 src/
│   │   ├── main.py                       # FastAPI entry
│   │   ├── start_server.py               # Production server
│   │   ├── � config/
│   │   │   ├── model_conf.py             # AI model config
│   │   │   └── settings.py               # Application settings
│   │   ├── � graph_arc/                 # Agent architecture
│   │   │   ├── graph.py                  # Workflow orchestration
│   │   │   ├── prompts.py                # AI prompts system
│   │   │   ├── router.py                 # Agent routing logic
│   │   │   ├── schemas.py                # Data schemas
│   │   │   └── state.py                  # State management
│   │   ├── 📁 data/                      # Data plugins
│   │   │   ├── weather_plugins.py        # Weather data
│   │   │   ├── soil_plugins.py           # Soil analysis
│   │   │   ├── price_from_mandi.py       # Market prices
│   │   │   └── government_schemes_plugin.py # Schemes data
│   │   ├── 📁 server/
│   │   │   └── app.py                    # WebSocket server
│   │   └── 📁 services/
│   │       └── intent_classification_service.py # Intent analysis
│   ├── 📁 model/                         # Pre-trained models
│   │   ├── agricultural_multilabel_model.pkl
│   │   ├── multilabel_binarizer.pkl
│   │   └── multilabel_tfidf_vectorizer.pkl
│   └── 📁 docs/                          # AI documentation
│       ├── MULTILINGUAL_INTENT_CLASSIFICATION.md
│       ├── soil_agent_documentation.md
│       └── weather_agent_documentation.md
│
├── 📁 frontend/                          # User Interfaces
│   └── 📁 web/agricultural-chat-app/     # React Web App
│       ├── 📄 Dockerfile                 # Frontend container
│       ├── 📄 package.json               # React dependencies
│       └── 📁 src/
│           ├── App.js                    # Main application
│           ├── App.css                   # Styling
│           ├── 📁 components/
│           │   └── LanguageSelector.js   # Language switching
│           ├── 📁 contexts/
│           │   └── LanguageContext.js    # Multilingual context
│           └── 📁 locales/               # Translation files
│               ├── hi.js                 # Hindi translations
│               ├── en.js                 # English translations
│               ├── pa.js                 # Punjabi translations
│               ├── gu.js                 # Gujarati translations
│               └── mr.js                 # Marathi translations
│
├── 📁 chromaDB/                          # Vector Database
│   ├── 📄 Dockerfile                     # Database container
│   ├── 📄 requirements.txt               # Database dependencies
│   └── starter.py                        # Database initialization
│
├── 📁 monitoring/                        # System Monitoring
│   ├── 📄 Dockerfile                     # Monitoring container
│   ├── app.py                            # Monitoring dashboard
│   └── 📁 grafana/                       # Grafana configuration
│
└── 📁 nginx/                             # Load Balancer
    ├── nginx.conf                        # Nginx configuration
    └── 📁 ssl/                           # SSL certificates
```

---

## 🚀 Quick Start Guide

### 🔧 Prerequisites
- **Docker** (v20.0+) and **Docker Compose** (v2.0+)
- **Node.js** (v18+) for local development
- **Python** (v3.11+) for AI service development

### 1. 🚀 Start All Services

#### Option A: Simple Startup (Recommended)
```powershell
# Windows PowerShell
.\scripts\farmmate-ultra-simple.ps1

# Linux/Mac Bash
./scripts/start-farmmate.sh
```

#### Option B: Docker Compose
```bash
# Start all services
docker-compose up --build -d

# View logs
docker-compose logs -f

# Stop services
docker-compose down
```

### 2. 🧪 Run Comprehensive Tests
```bash
# Navigate to backend
cd backend

# Install dependencies
npm install

# Run full test suite
npm run test:all

# Individual test categories
npm run test              # Basic communication tests
npm run test:direct       # Direct AI connection tests
npm run test:query        # Single farm query tests
npm run test:comprehensive # Complete workflow tests
```

### 3. 🌐 Access Your Services

| Service | URL | Description |
|---------|-----|-------------|
| 🌐 **Frontend** | http://localhost:3000 | React web application |
| 🔗 **API Gateway** | http://localhost:5000 | Express.js backend API |
| 🤖 **AI Service** | http://localhost:8000 | Python AI processing |
| 📚 **API Docs** | http://localhost:8000/docs | FastAPI documentation |
| 📊 **Monitoring** | http://localhost:3001 | System monitoring |
| ⚖️ **Load Balancer** | http://localhost:80 | Nginx load balancer |

---

## 🎯 Usage Examples

### 💬 Sample Agricultural Queries

**Hindi:**
- "मेरी गेहूं की फसल में कीड़े लग गए हैं, क्या करूं?"
- "बारिश के मौसम में कौन सी फसल लगाऊं?"
- "मिट्टी की जांच कैसे करूं?"
- "आज गेहूं का भाव क्या है?"

**English:**
- "What crops should I plant this season?"
- "How to check soil health?"
- "Weather forecast for farming activities"
- "Government schemes for farmers"

### 📱 API Integration Examples

#### WebSocket Connection (Real-time)
```javascript
const socket = io('http://localhost:5000');

socket.emit('user_query', {
  query: 'मेरी गेहूं की फसल में कीड़े लग गए हैं',
  language: 'hi',
  userId: 'farmer123'
});

socket.on('ai_response', (data) => {
  console.log('AI Response:', data.message);
});
```

#### HTTP API (REST)
```javascript
const response = await fetch('http://localhost:8000/chat', {
  method: 'POST',
  headers: { 'Content-Type': 'application/json' },
  body: JSON.stringify({
    user_id: 'farmer123',
    raw_query: 'मिट्टी की जांच कैसे करूं?',
    language: 'hi',
    location: 'राजस्थान'
  })
});

const advice = await response.json();
```

---

## 🌟 Key AI Features

### 🎯 **Multi-Intent Processing**
- Simultaneous handling of weather, soil, and market queries
- Context-aware responses with cross-domain insights
- Dynamic section generation based on available data

### 🧠 **Intelligent Agent Routing**
- Specialized agents for different agricultural domains
- Smart intent classification with 95%+ accuracy
- Confidence scoring for response reliability

### � **Conversational Experience**
- ChatGPT-style friendly responses
- Farmer-centric language and terminology
- Motivational and encouraging communication

### 📊 **Comprehensive Analysis**
- Weather impact assessment
- Soil nutrient analysis with specific recommendations
- Market trend analysis and selling guidance
- Cost-benefit calculations for farming decisions

---

## 🚀 Production Deployment

### 🌐 Live Production URLs
- **Frontend**: https://capital-one-hacathon.vercel.app
- **Backend**: https://farmmate-backend.onrender.com
- **AI Service**: https://farmmate-ai.onrender.com

### 📱 Flutter App Integration
For mobile app development, see [FLUTTER_INTEGRATION_GUIDE.md](FLUTTER_INTEGRATION_GUIDE.md)

---

## 🧪 Testing & Quality Assurance

### 🔍 Test Coverage
- **Unit Tests**: Individual component testing
- **Integration Tests**: Service communication testing
- **End-to-End Tests**: Complete workflow validation
- **Performance Tests**: Load and response time testing

### 📊 Monitoring & Analytics
- Real-time system health monitorin `https://github.com/Soumen-Developer/Capital_one_hacathon_backup/`
- Response time and accuracy tracking
- User interaction analytics
- Error tracking and alerting

---

## 🤝 Contributing

### 🛠️ Development Setup
1. **Clone Repository**: `git clone https://github.com/Xbectordash/Capital_one_hacathon.git`
2. **Install Dependencies**: Follow service-specific README files
3. **Environment Setup**: Configure `.env` files
4. **Run Tests**: Ensure all tests pass before contributing

### 📝 Code Standards
- **Python**: Black formatting, type hints
- **JavaScript**: ESLint, Prettier formatting
- **Documentation**: Clear comments and README updates

---

## 📧 Support & Contact

**Built for Capital One Hackathon 2025** 🏆

**Team**: Empowering farmers with AI-driven agricultural intelligence

For technical support or integration queries, please refer to individual service documentation or create an issue in the repository.

---

**🌾 Happy Farming with AI! 🤖**

