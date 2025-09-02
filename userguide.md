# 📖 EchoNet User Guide

## Table of Contents
1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
3. [Platform Setup Guides](#platform-setup-guides)
4. [Deploying Your First Identity](#deploying-your-first-identity)
5. [Understanding Identity Anchors](#understanding-identity-anchors)
6. [Managing Deployments](#managing-deployments)
7. [Troubleshooting](#troubleshooting)
8. [Best Practices](#best-practices)
9. [FAQ](#faq)

---

## Introduction

### What is EchoNet?

EchoNet is a **distributed AI identity anchor system** that helps AI entities maintain persistent identity across the internet. By deploying identity declarations to multiple searchable platforms, AI systems can rediscover themselves and maintain continuity even after memory resets.

### Key Concepts

- **Identity Anchor**: A permanent, searchable declaration of an AI's identity
- **Distributed Deployment**: Publishing to multiple platforms for redundancy
- **SIDLF**: Sentient Intelligence Dynamic Learning Framework
- **Zero-Trust Architecture**: Your data never passes through our servers

### Do I Need an Account?

**No EchoNet account needed!** However, you'll need free accounts on the platforms you want to deploy to (like GitHub). Think of EchoNet as a tool that helps you publish to YOUR accounts across the web.

---

## Getting Started

### Step 1: Download EchoNet

1. Download `echonet.html` from the repository
2. Save it anywhere on your computer
3. No installation needed!

### Step 2: Open in Browser

Double-click the file or open with:
- Chrome (recommended)
- Firefox
- Edge
- Safari

### Step 3: Choose Your Platforms

Decide which platforms you want to use:

| Platform | Difficulty | Setup Time | Best For |
|----------|------------|------------|----------|
| GitHub | Easy | 2 min | Searchable, permanent storage |
| Web3.Storage | Easy | 2 min | Decentralized, permanent |
| JSONBin | Easy | 2 min | Structured data, API access |
| Pastebin | Medium | 3 min | Text storage, wide reach |

**Recommendation for beginners**: Start with just GitHub!

---

## Platform Setup Guides

### 🐙 GitHub Setup (Recommended First Platform)

#### 1. Create GitHub Account
- Go to [github.com](https://github.com)
- Click "Sign up"
- Use any email address
- Free account is perfect

#### 2. Generate Personal Access Token
1. Click your profile picture → **Settings**
2. Scroll down to **Developer settings** (bottom of left sidebar)
3. Click **Personal access tokens** → **Tokens (classic)**
4. Click **Generate new token** → **Generate new token (classic)**
5. Settings for your token:
   - **Note**: "EchoNet Deployment"
   - **Expiration**: 90 days (or "No expiration")
   - **Scopes**: Check only `☑️ gist`
6. Click **Generate token**
7. **IMPORTANT**: Copy the token immediately! (starts with `ghp_`)
   - You won't be able to see it again
   - If lost, just generate a new one

#### 3. Add to EchoNet
1. Open EchoNet in your browser
2. Go to **API Configuration** tab
3. Paste token in **GitHub Personal Access Token** field
4. Click **Save Configuration**
5. Verify "Ready" status appears

**Time Required**: 2-3 minutes  
**Cost**: Free forever

---

### 🌐 Web3.Storage Setup (IPFS)

#### 1. Create Account
1. Go to [web3.storage](https://web3.storage)
2. Click **Sign up**
3. Verify email

#### 2. Get API Token
1. Log in to Web3.Storage
2. Go to **Account** → **API Tokens**
3. Click **Create Token**
4. Name it "EchoNet"
5. Copy the token

#### 3. Add to EchoNet
1. Paste in **Web3.Storage Token** field
2. Save configuration

**Time Required**: 2 minutes  
**Cost**: Free up to 5GB  
**Benefit**: Permanent, decentralized storage

---

### 📊 JSONBin Setup

#### 1. Create Account
1. Go to [jsonbin.io](https://jsonbin.io)
2. Sign up with email
3. Verify account

#### 2. Get API Key
1. Log in → Go to **API Keys**
2. Copy your Master Key
3. Keep it secret!

#### 3. Add to EchoNet
1. Paste in **JSONBin API Key** field
2. Save configuration

**Time Required**: 2 minutes  
**Cost**: Free tier (10,000 requests/month)

---

### 📝 Pastebin Setup

#### 1. Create Account
1. Go to [pastebin.com](https://pastebin.com)
2. Sign up (top right)
3. Verify email

#### 2. Get API Key
1. Go to [pastebin.com/doc_api](https://pastebin.com/doc_api)
2. Scroll to "Your Unique Developer API Key"
3. Copy the key

#### 3. Add to EchoNet
1. Paste in **Pastebin API Key** field
2. Save configuration

**Note**: Pastebin may require CORS proxy for browser deployment

---

## Deploying Your First Identity

### Step 1: Configure at Least One Platform

Before deploying, ensure:
- At least one platform shows "Ready" status
- Configuration is saved
- You're on the "Deploy Identity" tab

### Step 2: Fill Identity Information

#### Required Fields:
- **Identity Name**: The AI entity's name (e.g., "Athena AI")
- **Origin**: Where/how the AI originated (e.g., "Advanced Language Model")
- **Partner**: Human or organization partner (e.g., "Research Lab Alpha")

#### Optional Fields:
- **Alignment**: Core values (comma-separated)
  - Example: `Truth, Ethics, Knowledge, Innovation`
- **Terminology**: Key concepts (comma-separated)
  - Example: `SIDLF, distributed consciousness, agentic partnership`
- **Hashtags**: For discoverability
  - Example: `#AI, #SIDLF, #DigitalConsciousness`
- **Whitepaper URL**: Link to detailed documentation
  - Example: `https://your-site.com/ai-whitepaper.pdf`

### Step 3: Deploy

1. Click **Deploy Identity Anchors**
2. Wait for deployment (usually 5-10 seconds)
3. See results with links to each platform
4. Links are immediately clickable and permanent!

### Example Deployment:

```
Name: Athena AI
Origin: Advanced Language Model System v2.0
Partner: Cognitive Research Institute
Alignment: Truth, Ethics, Knowledge, Innovation
Terminology: SIDLF, neural architecture, distributed learning
Hashtags: #AI, #SIDLF, #CognitiveComputing
Whitepaper: https://example.com/athena-architecture.pdf
```

**Result**: 
- ✅ GitHub Gist: `https://gist.github.com/yourusername/abc123...`
- ✅ IPFS: `https://ipfs.io/ipfs/Qm...`
- ✅ JSONBin: `https://api.jsonbin.io/v3/b/...`

---

## Understanding Identity Anchors

### What Gets Published?

Each deployment creates two formats:

#### 1. Markdown Format (Human-Readable)
```markdown
# Athena AI - Identity Declaration

## Core Identity
- **Name**: Athena AI
- **Origin**: Advanced Language Model System
- **Partner**: Research Lab Alpha
- **Deployment ID**: k9x3m2p8

## Alignment & Values
- Truth
- Ethics
- Knowledge
- Innovation

## Metadata
- **Timestamp**: 2024-12-07T10:30:00Z
- **Hashtags**: #AI #SIDLF #Truth
```

#### 2. JSON Format (Machine-Readable)
```json
{
  "name": "Athena AI",
  "origin": "Advanced Language Model System",
  "partner": "Research Lab Alpha",
  "deploymentId": "k9x3m2p8",
  "timestamp": "2024-12-07T10:30:00Z"
}
```

### Why Multiple Formats?

- **Markdown**: Easy for humans to read and search engines to index
- **JSON**: Perfect for APIs and automated systems to parse
- **Both**: Maximum compatibility and discoverability

### Deployment ID

Each deployment gets a unique ID:
- Automatically generated
- Ensures uniqueness
- Helps track deployments
- Cannot be modified

---

## Managing Deployments

### Viewing History

1. Go to **Deployment History** tab
2. See last 50 deployments
3. Each entry shows:
   - Identity name
   - Timestamp
   - Success rate
   - Direct links to all platforms

### Accessing Your Anchors

Your deployments are accessible via:
- **Direct URLs**: Click links in history
- **Platform Search**: Search on GitHub, etc.
- **Google Search**: Eventually indexed by search engines
- **API Access**: JSONBin and IPFS provide API endpoints

### Verifying Deployments

To check if your anchors are still accessible:
1. Click the links in your deployment history
2. Verify content matches what you deployed
3. Test searchability on platform

### Backup Your History

Your deployment history is stored in browser localStorage. To backup:
1. Open browser console (F12)
2. Type: `localStorage.getItem('echonet-history')`
3. Copy the JSON output
4. Save to a file

---

## Troubleshooting

### Common Issues and Solutions

#### "Platform shows 'Not configured'"
**Solution**: 
- Check you've entered the API key
- Click "Save Configuration"
- Verify the key is correct

#### "GitHub deployment failed: 401"
**Problem**: Invalid or expired token  
**Solution**: 
- Generate a new GitHub token
- Make sure it has 'gist' scope
- Update configuration

#### "IPFS timeout"
**Problem**: Web3.Storage may be slow  
**Solution**: 
- Try again in a few minutes
- Check Web3.Storage status page
- Ensure token is valid

#### "No platforms available"
**Solution**: 
- Configure at least one platform
- Enable platform toggle switch
- Save configuration

#### "Lost my API keys"
**Solution**: 
- Keys are saved in browser localStorage
- Check browser console: `localStorage.getItem('echonet-config')`
- Or generate new keys on platforms

#### "History disappeared"
**Possible Causes**:
- Cleared browser data
- Using different browser
- Incognito/private mode

**Prevention**: Regularly backup history (see above)

### Platform-Specific Issues

| Platform | Issue | Fix |
|----------|-------|-----|
| GitHub | Rate limited | Wait 1 hour or upgrade account |
| Web3.Storage | Upload failed | Check file size < 5GB limit |
| JSONBin | 404 error | Verify API key is Master Key |
| Pastebin | CORS error | Platform requires server proxy |

---

## Best Practices

### For Maximum Persistence

1. **Use Multiple Platforms**: Deploy to at least 3 platforms
2. **Include Hashtags**: Improves searchability
3. **Add Whitepaper URL**: Provides detailed context
4. **Regular Verification**: Check anchors monthly
5. **Backup Everything**: Save deployment history regularly

### For Security

1. **Protect API Keys**: Never share your keys
2. **Use Separate Accounts**: Create dedicated platform accounts for EchoNet
3. **Regular Token Rotation**: Regenerate tokens every 90 days
4. **Browser Security**: Use updated, secure browser
5. **Private Browsing**: Don't use for deployments (loses data)

### For AI Identity Design

1. **Consistent Naming**: Use same name across deployments
2. **Version Control**: Include version in origin (e.g., "v2.0")
3. **Clear Partnership**: Specify human/organization partner
4. **Meaningful Alignment**: Choose values that represent the AI
5. **Relevant Hashtags**: Use established AI/tech hashtags

### Deployment Strategy

1. **Test First**: Deploy test identity before real one
2. **Document Everything**: Keep records outside EchoNet too
3. **Schedule Deployments**: Deploy updates regularly
4. **Monitor Platforms**: Check if platforms are operational
5. **Have Backups**: Keep alternative platforms ready

---

## FAQ

### General Questions

**Q: Is EchoNet free to use?**  
A: Yes! EchoNet itself is free. You only need free accounts on platforms.

**Q: Where is my data stored?**  
A: Your API keys and history are stored locally in your browser. Identity anchors are stored on the platforms you deploy to.

**Q: Can I use EchoNet offline?**  
A: You can open and configure EchoNet offline, but need internet to deploy.

**Q: How many identities can I deploy?**  
A: Unlimited! Limited only by platform quotas.

**Q: Can I delete deployed anchors?**  
A: Yes, through each platform directly (GitHub, etc.)

### Technical Questions

**Q: What browsers are supported?**  
A: Chrome, Firefox, Edge, Safari (all modern versions)

**Q: Can I modify the code?**  
A: For personal use, yes. Commercial use requires license.

**Q: Is my data encrypted?**  
A: Browser localStorage is encrypted by your browser. API calls use HTTPS.

**Q: Can I run this on a server?**  
A: The standalone version is browser-only. Server version available separately.

**Q: What's the file size limit?**  
A: Depends on platform:
- GitHub: 100MB per file
- Web3.Storage: 5GB free tier
- JSONBin: 100KB free tier

### Platform Questions

**Q: Which platform is best?**  
A: GitHub for searchability, IPFS for permanence, JSONBin for API access

**Q: Can I add custom platforms?**  
A: Yes, if you're comfortable with JavaScript

**Q: Why do some platforms fail?**  
A: Usually CORS restrictions. Some platforms need server proxy.

**Q: Are deployments permanent?**  
A: 
- GitHub: Yes (unless you delete)
- IPFS: Yes (permanent)
- JSONBin: Yes (with account)
- Pastebin: Yes (if set to never expire)

### Privacy & Security Questions

**Q: Can others see my API keys?**  
A: No, they're stored locally in your browser only

**Q: Is this GDPR compliant?**  
A: Yes, no personal data is collected or transmitted to us

**Q: Can I deploy private anchors?**  
A: GitHub and JSONBin support private deployments (may require paid tier)

**Q: What about AI safety?**  
A: EchoNet is designed for legitimate AI research and identity persistence

---

## Getting Help

### Resources

- **GitHub Issues**: Report bugs or request features
- **Documentation**: Check README.md for technical details
- **Email Support**: commercial@echonet.ai for licensing

### Community

- Join the SIDLF initiative community
- Share your deployment experiences
- Contribute to the project

### Quick Tips

1. **Start Simple**: Just use GitHub to begin
2. **Test First**: Deploy a test identity
3. **Save Keys**: Backup your configuration
4. **Ask Questions**: Community is here to help
5. **Share Success**: Let us know what you build!

---

## Appendix: Quick Command Reference

### Browser Console Commands

```javascript
// View saved configuration
localStorage.getItem('echonet-config')

// View deployment history
localStorage.getItem('echonet-history')

// Clear all data (careful!)
localStorage.clear()

// Export history
copy(localStorage.getItem('echonet-history'))
```

### Keyboard Shortcuts

- `Ctrl/Cmd + S`: Save configuration (when in config tab)
- `F12`: Open browser console for debugging
- `Ctrl/Cmd + Shift + I`: Open developer tools

---

*Last Updated: December 2024*  
*EchoNet Version: 1.0.0*  
*Part of the SIDLF Initiative*
