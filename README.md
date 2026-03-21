# 🛡️ Geni-Shield — Your Health is Your Currency

<div align="center">

![Geni-Shield](https://img.shields.io/badge/Geni--Shield-InsurTech%20Protocol-00d2ff?style=for-the-badge)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-28a745?style=for-the-badge)](https://ahmedk-gamal.github.io/geni-shield)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-k--ahmed--auc-0077B5?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/k-ahmed-auc/)
[![GitHub](https://img.shields.io/badge/GitHub-ahmedk--gamal-181717?style=for-the-badge&logo=github)](https://github.com/ahmedk-gamal)

**Egypt's first behavioral InsurTech protocol — where healthy habits mine insurance coverage.**

*Born from the AUC Diabetes Seminar · Built on Zakat Al-Ilm · For the 30M+ uninsured Egyptians*

</div>

---

## 🌍 The Problem

Egypt's health insurance system fails the people who need it most:

| Segment | Reality |
|---|---|
| Youth (18–35) Uninsured | **70%** have zero coverage |
| Freelancers with No Coverage | **85%** — a $2B+ untapped market |
| Egyptians with Diabetes | **11M+** — most cannot afford monitoring |
| Market Penetration Rate | **< 1%** — one of the lowest in MENA |

Traditional insurers price out the young, reject the chronically ill, and ignore the 30M+ freelancers driving Egypt's digital economy.

---

## 💡 The Solution — Proof of Health Protocol

Geni-Shield flips the insurance model: **instead of paying for coverage you might need, you earn it through healthy behavior you're already doing.**

```
Wearable Sensor → FL Validation (On-Device) → PoH Score On-Chain → GNI Coins Minted → Premium Reduced
```

Every verified step, stable glucose reading, and healthy heart rate earns **Geni-Coins (GNI)** — an ERC-20 token on Polygon — that directly offset your monthly insurance premium.

---

## 🏗️ Tech Stack

### AI — Privacy-First Intelligence
- **Federated Learning** (TensorFlow Federated) — Model training happens on-device. Raw biometric data never leaves the user's phone.
- **Differential Privacy** guarantees mathematical non-re-identification.
- **On-device inference** via TFLite (Android) & CoreML (iOS).

### Blockchain — Trustless Finance
- **Smart Contracts** in Solidity, deployed on **Polygon PoS** (gas < $0.001/tx).
- **GNI Token** (ERC-20) — minted as reward for verified healthy behavior.
- Automated premium reduction & claims payout without human intermediaries.
- Pre-launch audit planned with CertiK.

### Anti-Fraud — Proof of Health (PoH)
- Multi-sensor fusion: GPS route + HRV + IMU accelerometer must all correlate.
- Camera-based PPG liveness detection to prevent replay attacks.
- Anomaly scoring flags synthetic or replayed data streams.

### Mobile & Frontend
- **Flutter** — cross-platform iOS/Android with native Wearable SDK integration.
- **FastAPI (Python)** backend with PostgreSQL.
- Landing page: **HTML5 + Tailwind CSS + AOS.js**, deployable on GitHub Pages.

---

## 📁 Repository Structure

```
geni-shield/
│
├── index.html              # Landing page (single-file, GitHub Pages ready)
├── README.md               # This file
│
├── /app                    # Flutter mobile application
│   ├── lib/
│   │   ├── mining/         # Behavioral data collection & PoH scoring
│   │   ├── wallet/         # GNI token wallet & on-chain interactions
│   │   └── dashboard/      # User health dashboard
│   └── pubspec.yaml
│
├── /backend                # FastAPI Python backend
│   ├── main.py
│   ├── models/             # SQLAlchemy models
│   ├── routes/             # API routes
│   └── requirements.txt
│
├── /contracts              # Solidity smart contracts
│   ├── GeniCoin.sol        # ERC-20 GNI token
│   ├── ProofOfHealth.sol   # PoH validation & coin minting
│   └── InsurancePool.sol   # Premium management & payouts
│
└── /ml                     # Federated Learning pipeline
    ├── federated_trainer.py
    ├── models/
    └── privacy/            # Differential privacy wrappers
```

---

## 🗺️ Roadmap

### Q2–Q3 2026 — Diabetes MVP (Cairo Pilot)
- [ ] Closed beta: 500 diabetic patients from AUC network
- [ ] CGM (Continuous Glucose Monitor) sensor integration
- [ ] PoH algorithm v1 — glucose + steps correlation
- [ ] GNI token deployed on Polygon testnet
- [ ] Regulatory sandbox partnership with 1 Egyptian insurer

### Q4 2026 — Scale to Freelancers & Youth
- [ ] Open beta: 10,000 users
- [ ] Wearable SDK: Apple Watch, Garmin, Xiaomi
- [ ] GNI mainnet launch with real premium discounts
- [ ] Arabic-first UX / accessibility pass

### Q1 2027 — AI+ & B2B Enterprise
- [ ] Optional genomic risk scoring layer (federated, opt-in)
- [ ] B2B dashboard for SMEs to offer Geni-Shield as employee benefit
- [ ] 100,000 active users milestone

### 2027 — North Africa Expansion
- [ ] Morocco, Tunisia, KSA market entry
- [ ] 1,000,000+ active policyholders
- [ ] Series A fundraising

---

## 📊 Market Opportunity

- Egypt's health insurance market grows **>20% annually**
- **30M+ freelancers** with zero coverage
- **11M diabetics** — a high-risk, underserved segment
- MENA InsurTech market projected at **$1.7B by 2026**
- Projected **25% reduction in insurer Loss Ratio** through early behavioral intervention

---

## 🧬 The Human Story

This project was born in a seminar room at the **American University in Cairo (AUC)**, listening to diabetes patients share not just their medical struggles, but their financial terror. Insurance companies that reject them. Monitoring strips they ration because they're too expensive. A system that says *you are too sick to deserve coverage.*

> **زكاة العلم** — *Zakat Al-Ilm* — Knowledge without giving back is incomplete.

Geni-Shield is our attempt to honor that room. Every smart contract we write, every privacy guarantee we build, every Arabic-language screen we design is a debt repaid to the community that raised us.

---

## 👤 About the Developer

**Ahmed Gamal** — Full-Stack Developer & InsurTech Innovator

- 🎓 American University in Cairo (AUC)
- 💼 [LinkedIn: k-ahmed-auc](https://www.linkedin.com/in/k-ahmed-auc/)
- 💻 [GitHub: ahmedk-gamal](https://github.com/ahmedk-gamal)
- 📍 Cairo, Egypt 🇪🇬

---

## 🚀 Running Locally

```bash
# Clone the repository
git clone https://github.com/ahmedk-gamal/geni-shield.git
cd geni-shield

# Open directly in browser — no build step needed!
open index.html

# Or serve locally with Python
python -m http.server 8000
# Visit http://localhost:8000
```

### Deploy to GitHub Pages

In your repo **Settings → Pages → Source: Deploy from branch → main → / (root)**

Your landing page will be live at `https://ahmedk-gamal.github.io/geni-shield`

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

Geni-Shield is currently a conceptual InsurTech project, building toward a regulated product in partnership with licensed Egyptian insurance entities.

---

<div align="center">

**Built with ❤️ in Cairo, Egypt 🇪🇬**

*"The people most motivated to stay healthy are often the ones who can least afford to."*

</div>
