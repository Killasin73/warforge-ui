# 🔥 WARFORGE-UI

**AI-Powered Contract Compliance Dashboard**  
*React frontend for visualizing WARFORGE's real-time PDF risk assessments with DOD-grade security*

![WARFORGE-UI Demo](https://github.com/yourteam/warforge-ui/blob/main/docs/classified-demo.gif?raw=true)  
*Operational demo: [warforge.example.com/secure-demo](https://warforge.example.com/secure-demo) (CAC/PIV required)*

## 🚀 Key Features
- **Drag & Drop Analysis** - Process 500+ page contracts in <5s
- **Threat Heatmaps** - Interactive clause risk visualization
- **Compliance Scoring** - AI-generated ratings (0-100) with NIST SP 800-171 alignment
- **Audit Mode** - Redaction-ready evidence logging with chain-of-custody
- **Secure API Handshake** - JWT tokens with 15m rotation via PKI

## ⚡ Quick Start
```bash
# Clone with SSH authentication (DOD-compliant)
git clone git@github.com:yourteam/warforge-ui.git --config core.sshCommand="ssh -i $DEPLOY_KEY_PATH"
cd warforge-ui

# Install with integrity checks and vulnerability audit
npm ci --audit

# Configure environment
cp .env.example .env.local
echo "REACT_APP_API_URL=https://warforge-backend.example.com" >> .env.local

# Generate TLS cert for dev (one-time)
openssl req -x509 -newkey rsa:2048 -keyout key.pem -out cert.pem -days 365 -nodes

# Launch dev server with TLS
HTTPS=true SSL_CRT_FILE=cert.pem SSL_KEY_FILE=key.pem npm start
