# Smart Contract-Based sBTC Attack Detection and Defense Network

## Overview
This project implements an innovative security framework for monitoring and protecting sBTC transactions through automated threat detection and defense mechanisms. The system utilizes smart contracts on the Stacks blockchain to provide real-time security monitoring and autonomous response capabilities.

## 🎯 Project Goals
- Create an autonomous security monitoring system for sBTC transactions
- Implement sophisticated pattern-based attack detection
- Develop automated defense mechanisms
- Reduce reliance on external monitoring systems
- Enhance overall sBTC network security

## 🏗 Architecture

### Core Components
1. **Transaction Monitor**
   - Tracks transaction history per user
   - Monitors transaction volumes and patterns
   - Implements threshold-based detection
   - Records recent transaction history (last 10 transactions)

2. **Pattern Recognition System** [NEW]
   - Transaction velocity monitoring
   - Burst detection mechanism
   - Historical pattern analysis
   - Dynamic risk scoring
   - Global statistics tracking

3. **Risk Assessment Engine** [NEW]
   - Multi-factor risk calculation
   - Velocity-based risk analysis
   - Burst pattern detection
   - Combined risk scoring
   - Configurable risk thresholds

4. **Threat Detection System**
   - Pattern recognition for suspicious activities
   - Real-time threat assessment
   - Event logging and notification system
   - High-risk transaction handling

5. **Defense Mechanism**
   - Automated response triggers
   - Configurable defense strategies
   - Administrative override capabilities

## 🛠 Technical Stack
- **Smart Contract Language**: Clarity
- **Blockchain**: Stacks
- **Asset Focus**: sBTC

## 📦 Installation

### Prerequisites
- Stacks blockchain development environment
- Clarity CLI tools
- Node.js (for testing environment)

### Setup
1. Clone the repository:
```bash
git clone https://github.com/your-repo/sbtc-security-monitor.git
cd sbtc-security-monitor
```

2. Install dependencies:
```bash
clarinet install
```

3. Deploy the contract:
```bash
clarinet deploy
```

## 💻 Usage

### Contract Initialization
```clarity
(contract-call? .sbtc-security-monitor initialize-monitoring)
```

### Register Transaction
```clarity
(contract-call? .sbtc-security-monitor register-transaction tx-sender amount)
```

### Check Transaction History
```clarity
(contract-call? .sbtc-security-monitor get-transaction-history user-address)
```

### Risk Scoring System [NEW]
The system now includes sophisticated risk assessment mechanisms:

1. **Velocity Risk**
```clarity
;; Monitors transaction volume over time
(calculate-velocity-risk recent-transactions)
```

2. **Burst Risk**
```clarity
;; Detects rapid succession transactions
(calculate-burst-risk recent-transactions)
```

3. **Combined Risk Score**
- Aggregates multiple risk factors
- Scale: 0-100 (100 being highest risk)
- Threshold configurations available

## 🔐 Security Features

### Current Implementation
- Transaction volume monitoring
- Advanced pattern recognition [NEW]
- Risk scoring system [NEW]
- Suspicious activity logging
- Administrative controls
- Global statistics tracking [NEW]

### Pattern Recognition Features [NEW]
1. **Velocity Monitoring**
   - Tracks transaction speed and volume
   - Configurable time windows
   - Dynamic threshold adjustment

2. **Burst Detection**
   - Identifies rapid transaction sequences
   - Customizable burst thresholds
   - Time-window analysis

3. **Historical Analysis**
   - Maintains recent transaction history
   - Pattern matching algorithms
   - Trend analysis

## 🚀 Development Roadmap

### Phase 1: Foundation ✓
- Basic monitoring system
- Transaction history tracking
- Simple threshold detection

### Phase 2: Enhanced Detection [CURRENT]
- ✓ Advanced pattern recognition
- ✓ Historical analysis
- ✓ Risk scoring system
- ⚡ Integration with global statistics
- ⚡ Machine learning preparation

### Phase 3: Automated Defense [UPCOMING]
- Smart response mechanisms
- Network protection protocols
- Recovery procedures

## 🤝 Contributing
Contributions are welcome! Please read our contributing guidelines before submitting pull requests.

### Branch Structure
- `main`: Production-ready code
- `develop`: Development branch
- Feature branches: `feature/pattern-recognition`, `feature/risk-scoring`, etc.

### Testing Requirements [NEW]
1. **Unit Tests**
   - Risk calculation functions
   - Pattern recognition algorithms
   - Transaction history management

2. **Integration Tests**
   - End-to-end transaction flow
   - Risk assessment pipeline
   - Pattern detection accuracy

## ⚠️ Security Considerations
- Contract requires thorough security audit before mainnet deployment
- Administrative functions restricted to authorized addresses
- Regular monitoring of threshold parameters recommended
- Risk scoring parameters should be carefully calibrated
- Pattern recognition thresholds require periodic review [NEW]
- Global statistics should be monitored for manipulation attempts [NEW]

## 📊 Monitoring and Analytics [NEW]
The system now provides:
- Transaction velocity metrics
- Risk score distribution
- Pattern detection statistics
- Global network statistics
- High-risk account tracking

## 📄 License
This project is licensed under the MIT License.

## 🤝 Contact
- Project Maintainer: Adigun Rasheed
- Email: adigun_olami99@yahoo.com
- GitHub: Raoshwill99

## Acknowledgments
- Stacks Foundation
- Bitcoin Community
- sBTC Working Group
