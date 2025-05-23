
🌐 Celo Skill-Sharing dApp
A peer-to-peer skill-sharing platform on the Celo blockchain with a sleek, notification-free UI — optimized for CodePen deployment.


📋 Table of Contents
Overview

Features

Smart Contract

Technical Details

Setup Instructions

Usage

Deployment

Troubleshooting

Contributing

License

Acknowledgments

🧩 Overview
The Celo Skill-Sharing dApp enables users to exchange services and skills using credits on a decentralized platform. With support for registration, service requests, reputation tracking, and on-chain contracts, it builds a trusted skill-exchange community.

The front-end is built as a single HTML file for CodePen or Vercel, styled with a yellow-to-purple gradient, purple headline with an underscore, and a clean, notification-free interface.

🚀 Features
👤 User Registration — Get started with 10 free credits.

📚 Skill Sharing — Register skills and assign credit cost (1–1000).

📩 Request Services — Select a skill and request a service.

✅ Complete Tasks — Providers mark requests as complete.

⭐ Rate Providers — Feedback via 0–5 rating system.

🧾 Profile Overview — View credits, reputation, and level.

🛑 Pause Contract — Owner-only control for platform toggling.

📋 Explore Skills — Responsive grid listing skill details.

✨ UI Highlights
Yellow-to-purple gradient background: #F6E05E → #6B46C1

Purple Celo Skill-Sharing title with a 60px underscore

Yellow Connect Wallet and purple action buttons with gradients

Poppins font, rounded corners, backdrop blur, and animations

Mobile responsive, single-file HTML

No notifications — all errors logged in the browser console

🛠 Smart Contract
Interacts with SkillSharing.sol deployed on Celo Mainnet:

Address: 0x47de9ef23d84fd68e586d80df9b5fc0008a108f2

RPC: https://forno.celo.org

🔑 Key Functions
registerUser()

registerSkill(name, credits)

requestService(skillId)

completeService(requestId)

rateProvider(requestId, rating)

setPaused(_paused)

getSkill(skillId)

getUserProfile(user)

Emits events for transparency: UserRegistered, SkillRegistered, ServiceRequested, ServiceCompleted, ReputationUpdated, Paused.

⚙️ Technical Details
Blockchain: Celo Mainnet (Chain ID: 42220)

Front-End:

Pure HTML/CSS/JS (single file)

Web3.js v1.7.5 via CDN

Poppins font via Google Fonts

No npm/node required

UI Stack:

Gradient background, backdrop blur, animations

MetaMask + Web3.js for wallet connection and signing

All dependencies via CDN

🧰 Setup Instructions
✅ Prerequisites
Browser: Chrome/Firefox with MetaMask

MetaMask Configuration:

yaml
Copy
Edit
Network: Celo Mainnet
RPC: https://forno.celo.org
Chain ID: 42220
Currency: CELO
CELO for gas: Buy or use Celo Faucet

⚡ Run on CodePen
Open CodePen

Create a new Pen

Paste index.html contents into the HTML section

Save and open with MetaMask connected to Celo

🖥️ Local Development
bash
Copy
Edit
git clone https://github.com/your-username/celo-skill-sharing.git
cd celo-skill-sharing
open index.html
🧪 Usage
🔗 Connect Wallet
Click Connect Wallet

Address appears on success

👤 Register as User
Click Register as User → receive 10 credits

🛠 Share a Skill
Enter name + credit cost → Register Skill

📩 Request Service
Browse available skills

Enter Skill ID → Request Service

✅ Complete Service
Enter Request ID → Complete Service

⭐ Rate Provider
Enter Request ID + rating (0–5) → Rate Provider

📊 View Profile
Shows credits, reputation, and level

🛑 Toggle Contract (Owner only)
Click Toggle Pause

🔍 All errors are shown in the browser console (F12 > Console)

🚀 Deployment
📌 CodePen (Quick Start)
Paste index.html into CodePen

Share the URL for feedback

🌐 Vercel (Static Hosting)
bash
Copy
Edit
# Project structure:
celo-skill-sharing-frontend/
└── index.html

# Deploy
git add index.html
git commit -m "Initial deploy"
git push origin main
Deploy via Vercel

🧯 Troubleshooting
Issue	Solution
No skills loaded	Check console, confirm MetaMask is on Celo, and contract is accessible
Tx fails	Ensure wallet has CELO and contract is not paused
Wallet issues	Reconnect MetaMask or switch accounts
Debugging	All logs appear in console; confirm ABI and node sync at forno.celo.org

🤝 Contributing
We welcome contributions! 🙌

bash
Copy
Edit
# Fork & create a feature branch
git checkout -b feature/your-feature

# Make changes, test, then commit
git add .
git commit -m "Add feature"
git push origin feature/your-feature
Open a pull request with a clear description

Follow the Code of Conduct

Preserve:

Notification-free UX

CodePen compatibility (single HTML file)

📄 License
This project is licensed under the MIT License.

🙏 Acknowledgments
Celo Community

Web3.js

Google Fonts

CodePen

Vercel

📌 Notes
Screenshot: Replace the placeholder with a real dApp screenshot.

Repo Structure:

index.html

LICENSE

CODE_OF_CONDUCT.md (optional)

Enhancements Ideas:

Skill search or filter

Visual cues for errors (border highlight)

Live demo badge

Walkthrough video

📢 Spread the Word
“Explore the Celo Skill-Sharing dApp with a sleek, notification-free UI! [GitHub URL] #Celo” — @CeloOrg
