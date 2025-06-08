# 🔥 WARFORGE-UI

**Tactical Contract Analysis Dashboard**  
*React frontend for real-time PDF compliance assessment with DoD Zero-Trust architecture*

![Classified Demo](https://github.com/yourteam/warforge-ui/blob/main/docs/secure-demo.gif?raw=true)  
*Operational demo: [warforge.example.com/secure-demo](https://warforge.example.com/secure-demo) (CAC/PIV + SIPRNet access required)*

## ⚡ Quick Start
```bash
# Clone with military-grade authentication
git clone git@github.com:yourteam/warforge-ui.git --config core.sshCommand="ssh -i $DEPLOY_KEY_PATH"
cd warforge-ui

# Install with cryptographic integrity verification
npm ci --audit

# Configure operational environment
cp .env.example .env.local
echo "REACT_APP_API_URL=https://warforge-backend.smil.mil" >> .env.local

# Generate FIPS 140-3 compliant TLS cert
openssl req -x509 -newkey rsa:3072 -keyout key.pem -out cert.pem -days 30 -nodes -sha384

# Launch secure dev environment
HTTPS=true SSL_CRT_FILE=cert.pem SSL_KEY_FILE=key.pem npm start

# Build for hardened production
npm run build
