# 🔥 WARFORGE-UI

**AI-Powered Contract Compliance Dashboard**  
*React frontend for visualizing WARFORGE's real-time PDF risk assessments with DOD-grade security*

![WARFORGE-UI Demo](https://github.com/yourteam/warforge-ui/blob/main/docs/demo.gif?raw=true)  
*Live classification demo: [warforge.example.com/classified-demo](https://warforge.example.com/classified-demo)*

## 🚀 Key Features
- **Drag & Drop Analysis** - Process 500+ page contracts in <5s
- **Threat Heatmaps** - Interactive clause risk visualization
- **Compliance Scoring** - AI-generated ratings (0-100) with NIST alignment
- **Audit Mode** - Redaction-ready evidence logging
- **Secure API Handshake** - JWT tokens with 15m rotation

## ⚡ Quick Start
```bash
# Clone with SSH authentication (DOD-compliant)
git clone git@github.com:yourteam/warforge-ui.git --config core.sshCommand="ssh -i $DEPLOY_KEY_PATH"
cd warforge-ui

# Install with integrity checks
npm ci --audit

# Configure environment (see .env.example for all options)
cp .env.example .env.local
echo "REACT_APP_API_URL=https://warforge-backend.example.com" >> .env.local

# Launch secure dev server (HTTPS)
npm run start:secure
