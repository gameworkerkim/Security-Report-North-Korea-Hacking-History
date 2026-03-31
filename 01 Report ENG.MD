# 🇺🇸 North Korea's Hacking Units — From Online Games to Cryptocurrency

> **SECURITY REPORT · APT / DPRK · 2025.03**  
> The Evolution of Cyber Attack Organizations Under the Reconnaissance General Bureau — Threat Analysis & Defense Guide

---

| Estimated Total Stolen | APT Attacks (South Korea, 2025) | Estimated Hacker Workforce | Global Crypto Hack Share |
|:---:|:---:|:---:|:---:|
| **$6.75B+** | **86 incidents** | **7,000+** | **60%** |

---

## Table of Contents

1. [North Korea's Hacking Organization Structure](#1-organization-structure)
2. [History of Hacking — From Game Bots to Central Banks](#2-history-of-hacking)
3. [Upbit Hack — A Turning Point Targeting Crypto](#3-upbit-hack)
4. [Infiltration via Telegram and Crypto Communities](#4-telegram-infiltration)
5. [Developer Impersonation — The Most Sophisticated Social Engineering Attack](#5-developer-impersonation)
6. [Bybit Hack — The Largest Single Crypto Theft in History](#6-bybit-hack)
7. [Money Laundering Methodology and Tracking Limitations](#7-money-laundering)
8. [Key Observations — AI Advancement and Industrialization of Attacks](#8-key-observations)
9. [Defensive Checklist for Individuals and Enterprises](#9-defensive-checklist)
10. [References](#references)

---

## 1. Organization Structure

North Korea's cyberattacks are not the work of individuals or private groups. They are a systematic, state-level cyber force operating directly under the **Reconnaissance General Bureau (RGB) of the Korean Workers' Party**. Established in 2009 by merging the Party's Operations Department, Bureau 35, and the Military's Reconnaissance Bureau, the RGB is composed of six directorates and directly commands the core hacking units.

> ⚠️ **The Significance of State-Sponsored Hacking**  
> These are not mere criminal gangs — they receive state funding and military technology support. The United Nations Security Council has repeatedly confirmed that funds stolen through hacking are diverted to finance nuclear weapons and ballistic missile development.

### Major Hacking Units

| Unit | Alias | Primary Mission | Notable Attacks |
|---|---|---|---|
| **Lazarus** | Zinc / Hidden Cobra | Financial theft, infrastructure destruction, broad APT | Sony Pictures, Upbit, Bybit |
| **Bluenoroff** | Lazarus sub-group | Specialist financial institution and crypto exchange theft | Bangladesh Bank, SWIFT attacks |
| **Andariel** | Silent Chollima | Ransomware, credential theft, defense industry hacking | Upbit conspiracy, 10+ defense contractors breached |
| **Kimsuky** | Thallium | Intelligence gathering, spear phishing, diplomatic/security secrets | KHNP hack, diplomatic network infiltration |
| **Scarcruft** | APT37 | Civilian/public sector infiltration in Korea, Japan, Middle East | Thae Yong-ho smartphone hack |

> 📊 AhnLab 2025 Report: North Korea's APT attacks (86 cases) far exceed China (27) and Russia (18).

---

## 2. History of Hacking

North Korea's hacking strategy evolved in stages — from selling game automation software for foreign currency in the early days, to infiltrating financial networks, deploying global ransomware, and ultimately stealing cryptocurrency.

### 📅 Timeline

**Early 2000s — Online Game Bot Programs (First Foreign Currency Scheme)**  
Via Korea Computer Center and Ryonghakdo Trading Corporation, North Korea developed and sold automation (bot) programs for games like Lineage, MapleStory, and Dungeon & Fighter. Revenues flowed through Bureau 39 into the ruling fund. One private server operator was arrested under the National Security Act after purchasing hacking tools from North Korean hackers and sending KRW 23.8 million to a Chinese bank account.

**2009 — Operation Troy**  
Targeting South Korean and US Forces Korea military. Malware lay dormant for at least four years collecting military intelligence from government and military computers. DDoS attacks simultaneously hit the Blue House website.

**2014 — Sony Pictures Hack / KHNP Hack**  
Sony Pictures was breached in retaliation for the film *The Interview* (depicting Kim Jong-un's assassination), destroying internal networks. The FBI officially named North Korea as the perpetrator. Domestically, blueprints of nuclear power plants at Korea Hydro & Nuclear Power were stolen.

**2016 — Bangladesh Bank Heist `$81M stolen`**  
SWIFT payment systems were hacked to issue fraudulent wire transfer instructions to the US Federal Reserve. Funds were laundered through Philippine casinos. Attributed to Bluenoroff.

**2017 — WannaCry Ransomware `[CRITICAL]`**  
300,000 computers infected across 150 countries. UK National Health Service paralyzed. Exploited the NSA-leaked EternalBlue vulnerability. US and UK governments officially blamed North Korea.

**2019 — Upbit Ethereum Theft `$52M stolen (KRW 58 billion)`**  
342,000 ETH stolen. After five years of investigation, confirmed as a joint operation by Lazarus and Andariel. Current market value: approximately KRW 1.47 trillion.

**2024 — All-Out Assault on Defense Contractors**  
Three units (Lazarus, Andariel, Kimsuky) deployed simultaneously. 83 defense companies targeted; 10+ successfully breached.

**2025 — Bybit Hack `$1.46B stolen`**  
A single developer's PC infection led to the largest single crypto theft ever. North Korea's 2025 total crypto theft surpassed $2 billion.

---

## 3. Upbit Hack

The November 2019 Upbit hack marked a decisive strategic pivot from traditional finance to **cryptocurrency exchanges**.

```
[Incident Summary]
Stolen    : 342,000 ETH (~$52M at the time / ~$1.47T KRW at current price)
Date      : November 2019
Confirmed : November 2024 (National Investigation Headquarters, Korea National Police)
Perpetrators: Lazarus + Andariel (joint operation)
Investigation: FBI cooperation; North Korean IPs and vocabulary ('heolhan il') confirmed
```

### Post-Theft Money Laundering Route

1. **North Korean Proprietary Exchanges (57%)** — ETH converted to BTC at 2.5% below market rate via 3 anonymous exchanges designed and operated by North Korea. No external KYC required; instantly cashed out.
2. **51 Exchanges Across 13 Countries (43%)** — Funds dispersed through exchanges in China, the US, Hong Kong, Switzerland, etc. to obscure origins and complicate international tracking.
3. **Chinese OTC Brokers and Underground Finance** — Converted to fiat currency via UnionPay card-linked accounts. Final cash-out with collaboration from organized crime groups such as the Triads.

---

## 4. Telegram Infiltration

Telegram's encrypted messaging, anonymity, and bot automation have made it a primary communication channel for the crypto community — and North Korea's key vector for deploying malware and reaching victims.

| Method | Description |
|---|---|
| **Fake Wallet App Distribution** | The 'Somora' app — a clone of MyEthereum's UI — distributed via Telegram links. Bypasses security checks by avoiding official app stores. |
| **Fake Investment Channels** | Builds trust via high-yield investment proposals in channels/DMs, then directs victims to install a 'dedicated platform' (malicious app). |
| **Zoom Meeting Impersonation** | Impersonates a contact on Telegram → sets up Calendly meeting → sends fake Zoom invite → instructs victim to run 'Zoom SDK update script'. Malicious code hidden under 10,000 blank lines. |
| **AI Deepfake Identity Fraud** | AI-generated fake faces and IDs used to impersonate investors or public figures. Difficult to detect even in live video calls. |

### Malware Capabilities (NimDoor Family)

```
Keylogging        : Records all keystrokes → steals passwords and seed phrases
Clipboard Monitor : Replaces copied wallet addresses with attacker's addresses in real time
Browser Data      : Steals stored credentials, cookies, and sessions
Wallet Extensions : Steals data from 24+ wallet extensions including MetaMask
Remote Control    : Remotely controls webcam and microphone; transfers or deletes files
Telegram Data     : Runs script (tlgrm) to exfiltrate local Telegram data
Persistence       : Registers LaunchAgent (macOS) to auto-execute after reboot
```

---

## 5. Developer Impersonation

The most prominent tactic in 2024–2025 is **posing as IT developers or engineers and obtaining legitimate employment at crypto firms**. According to a Chainalysis report, more than 12 crypto companies in 2024 alone were infiltrated by North Korean operatives as legitimate employees.

> ⚠️ **The Neutralization of Perimeter Security**  
> When an attacker already holds legitimate internal access, firewalls and network perimeter defenses are rendered ineffective. This strategy creates a fundamental trust crisis across the entire industry.

### Attack Stages

1. **Building a Fake Identity** — Combine AI-generated photos, fabricated work history, and ghost company references. Build an activity history on LinkedIn and GitHub over time.
2. **Applying for Remote Positions** — Target high-demand roles such as blockchain developer or smart contract engineer. Possess skills sufficient to pass technical interviews.
3. **Internal Reconnaissance** — While working as a legitimate employee, quietly map internal infrastructure, security architecture, and private key management over months.
4. **Execution — Assisting the Attack from Inside** — Provide credentials, disable security systems, approve fraudulent transactions to directly support the external hacking team.

### Malicious Open Source Attack via GitHub

```
// Attack Flow (Exploiting VSCode Automation)
Step 1: Upload a malicious repository disguised as a legitimate open-source project to GitHub
Step 2: Developer clones the repo and opens the folder in VSCode
Step 3: .vscode/tasks.json automatically executes the malicious script
Step 4: Malware payload disguised as .woff2 or .svg files to bypass security scans
Step 5: Exfiltrates browser credentials + data from 24+ wallet extensions
// Target OS: Windows / macOS / Linux — all covered
```

---

## 6. Bybit Hack

> *"Seventeen days after infecting one developer's MacBook, North Korea's Lazarus stole $1.5 billion through a single compromised node."*  
> — BlockEden Analysis Report, February 2026

| Item | Details |
|---|---|
| **Overview** | Occurred February 2025. ~$1.46 billion stolen from Bybit, the world's third-largest exchange. Largest single-incident theft in crypto history. |
| **Infiltration Method** | Developer's PC at Safe{Wallet} infected → backdoor inserted into multi-sig wallet signing infrastructure → multi-sig approval process manipulated. |
| **Laundering Speed** | $200–300M laundered within 48 hours of theft. 86.29% of stolen ETH converted to BTC within one month. |
| **Attribution** | FBI officially identified Lazarus affiliate **TraderTraitor**. Matches known North Korean network patterns and laundering methods. |

---

## 7. Money Laundering

| Method | Details |
|---|---|
| **Smurfing** | Transfers split into amounts under $500K and sent thousands of times to defeat international surveillance systems. |
| **Cross-chain Bridges / Tornado Cash** | Breaks the traceability chain by moving assets across different blockchains. Tornado Cash (OFAC-sanctioned) continues to be used via workarounds. |
| **Via Binance** | ICIJ investigation confirmed approximately $900M in North Korean hack proceeds flowed through 5 Binance accounts. |
| **Chinese Underground Finance** | Assets converted to fiat via OTC brokers, Triad networks, and Macau casinos. Chinese domestic networks remain the biggest tracking obstacle. |

---

## 8. Key Observations

| Change | Details |
|---|---|
| **① Precision Over Volume** | Hack count down 74%, total amount stolen up 51%. TRM Labs named this the "industrialization of crypto theft." |
| **② Exploiting Human Vulnerabilities** | Full shift from technical exploits to social engineering. Humans are more exploitable than code. Fake hiring and spear phishing are primary methods. |
| **③ Full AI Integration** | Deepfake identities, automated phishing documents, automated vulnerability scanning, webcam/microphone remote surveillance. AI is embedded across the entire attack lifecycle. |
| **④ World-Class Hacker Talent** | Swept 1st–4th place at HackerEarth competition; 18 wins at CodeChef from 2013–2020. Over 15 years of intensive recruitment and training. |

---

## 9. Defensive Checklist

> 💡 **Core Principle**: North Korea's attacks target human trust and habits more than technical vulnerabilities. Technical security measures must be paired with a security culture centered on people, processes, and supply chain integrity.

### Basic Defense Practices

- [ ] **Telegram DMs**: Never respond to investment proposals, files, or links from unknown contacts. Always verify the identity of apparent contacts through a separate channel.
- [ ] **Hardware Wallet**: Store significant assets in cold storage. Keep only small amounts for daily transactions in hot wallets.
- [ ] **Clipboard Hijacking**: Always visually verify the full wallet address immediately before sending. Use a clipboard monitoring security solution.
- [ ] **Job Offer Emails**: Immediately refuse any request to run task files. Verify identity through official channels.
- [ ] **Open Source Code**: Manually review `.vscode/tasks.json` and `package.json` scripts before execution. Disable VSCode auto-run.
- [ ] **Supply Chain Audit**: Regularly audit third-party libraries and services. Conduct thorough background checks when hiring contract developers.

### Two-Factor Authentication (2FA) — Last Line of Defense Against Account Takeover

> 🔐 **An Account Without 2FA Is a Safe Without a Lock**  
> Even if a password is stolen, an attacker cannot enter an account protected by 2FA without passing a second verification step.

| Method | Security Level | Description |
|---|---|---|
| **Hardware Security Key (FIDO2/U2F)** | 🟢 Strongest | Physical keys like YubiKey. If entered on a phishing site, the domain mismatch prevents authentication entirely. Strongly recommended for exchanges and high-value accounts. |
| **TOTP App (Google Authenticator / Authy)** | 🟡 Recommended | 6-digit OTP refreshed every 30 seconds. Safer than SMS and works offline. Store backup codes offline. |
| **SMS 2FA** | 🟠 Not Recommended | Vulnerable to SIM-swapping and SS7 protocol exploits. Replace with TOTP or a hardware key immediately. |
| **Email 2FA** | 🔴 Do Not Use | Email accounts are already primary phishing targets. Email 2FA is instantly nullified when the email account is compromised. |

**2FA Priority Order:** Exchange accounts > Email accounts > Telegram/Social media > Cloud storage  
For exchange API keys: always restrict to **withdrawal disabled / read-only** permissions + IP whitelist.

### PC Cafes and Public Internet — Never Access Crypto

> ⛔ **4 Threats When Using Public Computers**
> 1. **Keyloggers Cannot Be Detected** — Malware or keyloggers may already be installed and are invisible to the naked eye.
> 2. **Browser Sessions Linger** — Even after logging out, authentication data can remain in cache and cookies, exposed to the next user.
> 3. **Man-in-the-Middle Attack (MITM)** — On open networks (cafes, libraries, airports), attackers on the same network can intercept traffic or redirect you to a rogue access point.
> 4. **Shoulder Surfing** — Seed phrases and passwords entered in public may be seen by bystanders or captured by CCTV.

**✅ Rules to Follow:**
- [ ] Access crypto exchanges and wallets only from your own personal device (smartphone or laptop)
- [ ] If you must use a public PC, never enter seed phrases, private keys, or passwords
- [ ] Use a trusted, paid VPN before connecting to public Wi-Fi
- [ ] Install exchange apps only from official app stores — never via QR code or link
- [ ] Never expose your 2FA codes during screen sharing or livestreaming (streamers/YouTubers take special care)

**❌ Never Do This:**
- Rely solely on clearing browser history after using a PC cafe (useless if a keylogger is installed)
- Access a personal wallet or exchange over a PC cafe's LAN without a personal hotspot
- Log into an exchange on someone else's device ("just a quick look")

### Checklist for Exchange and Project Operators

**✅ Must Implement:**
- [ ] Limit hot wallet assets to no more than 10% of total; keep the rest in cold storage
- [ ] Audit security of the multi-sig wallet signing infrastructure itself — including third-party services (Bybit lesson)
- [ ] Enforce FIDO2 hardware key-based 2FA on all admin accounts
- [ ] Implement additional identity verification procedures for remote hires, accounting for deepfake risk
- [ ] Monitor internal access logs in real time and configure immediate alerts for anomalous behavior
- [ ] Deploy endpoint security solutions on developer machines; restrict installation of external software

**❌ Strictly Prohibited:**
- Deploying SDKs or libraries from unverified sources directly to production
- Processing large withdrawal requests via automated systems alone (no human verification step)
- Approving transactions without real-time cross-referencing against North Korea-sanctioned blockchain address databases

---

## References

All statistics, events, and claims in this report are based on the public sources listed below. Items where investigation results remain unconfirmed are described within the scope of information publicly available at the time of writing.

### Government and Law Enforcement

| # | Institution | Document | Date | URL |
|---|---|---|---|---|
| [1] | Korea National Police Agency | Upbit Hack Investigation Results (Lazarus & Andariel confirmed) | Nov 2024 | [Link](https://www.police.go.kr/www/news/press/2024/press2024111301.jsp) |
| [2] | KNPA / DAPA / NIS | Joint Inspection Results: Cyberattacks on Defense Contractors | Apr 2024 | [Link](https://www.boannews.com/media/view.asp?idx=129172) |
| [3] | FBI | TraderTraitor: North Korean Cyber Group Identified as Bybit Hack Perpetrator | Feb 2025 | [Link](https://www.fbi.gov/news/press-releases/fbi-identifies-north-korean-cyber-actors-responsible-for-bybit-hack) |
| [4] | OFAC | Sanctions Designations: Lazarus Group, Bluenoroff, Andariel | Sep 2019 | [Link](https://ofac.treasury.gov/recent-actions/20190913) |
| [5] | UN Security Council | Final Report of Panel of Experts, S/2024/215 | 2024 | [Link](https://www.undocs.org/S/2024/215) |
| [6] | NIS (Korea) / BfV (Germany) | Joint Cyber Threat Report on Lazarus Group | 2024 | [Link](https://www.nis.go.kr:4016/AF/1_7_3_1/view.do?seq=120) |

### Security Firms and Blockchain Analytics

| # | Organization | Document | Date | URL |
|---|---|---|---|---|
| [7] | Chainalysis | Crypto Crime Report 2025 | 2025 | [Link](https://www.chainalysis.com/blog/2025-crypto-crime-report/) |
| [8] | Elliptic | North Korea Crypto Theft: $2.02B in 2025 | Oct 2025 | [Link](https://www.elliptic.co/blog/north-korea-crypto-theft-2025) |
| [9] | TRM Labs | Bybit Hack Fund Tracking & TraderTraitor Attribution Report | Feb–Mar 2025 | [Link](https://www.trmlabs.com/blog/trm-insights-bybit-hack) |
| [10] | AhnLab | 2025 Cyber Threat Trends & 2026 Security Outlook | Nov 2025 | [Link](https://www.ahnlab.com/ko/site/securityinfo/secunews/secuNewsView.do?seq=73792) |
| [11] | Kaspersky | Lazarus Telegram Malware Distribution Report (Somora Analysis) | Jan 2020 | [Link](https://securelist.com/lazarus-on-the-hunt-for-big-game/97757/) |
| [12] | SentinelOne | NimDoor Malware Analysis — North Korea-Linked macOS Backdoor | Jul 2025 | [Link](https://www.sentinelone.com/blog/nimdoor-north-korea-linked-backdoor/) |
| [13] | BlockEden.xyz | Lazarus Group Playbook: Inside North Korea's $6.75B Crypto Theft | Feb 2026 | [Link](https://blockeden.xyz/ko/blog/2026/02/03/lazarus-group-playbook-north-korea-crypto-theft-6-75-billion/) |

### Media and Investigative Journalism

| # | Outlet | Article | Date | URL |
|---|---|---|---|---|
| [14] | ICIJ | North Korean Hack Proceeds Laundered Through Binance — $900M Confirmed | Nov 2025 | [Link](https://www.sedaily.com/NewsView/2H0HNUR6GO) |
| [15] | Radio Free Asia (RFA) | Bybit Hack Laundering Traced — Interview with TRM Labs Policy Director | Mar 2025 | [Link](https://www.rfa.org/korean/in-focus/2025/03/13/north-korea-bybit-hack-crypto-laundering/) |
| [16] | Sisa Journal | Kim Jong-un's Secret Weapon: The Reality of North Korea's Hacker Units | Nov 2024 | [Link](https://www.sisajournal.com/news/articleView.html?idxno=316144) |
| [17] | SBS News | North Korean Malware Disguised as Crypto App Spreading via Telegram | Dec 2022 | [Link](https://news.sbs.co.kr/news/endPage.do?news_id=N1007009050) |
| [18] | Seoul Shinmun | North Korea's Massive AI-Powered Cyber Assault on Korea | Nov 2025 | [Link](https://www.seoul.co.kr/news/economy/industry/2025/11/30/20251130500108) |
| [19] | Herald Economy | Shift from Scatter-Shot to 'Big Score': North Korea's Evolving Crypto Strategy | Dec 2025 | [Link](https://biz.heraldcorp.com/article/10640660) |
| [20] | Daily Secu | North Korea's Lazarus Group: Crypto Theft Surpasses $3 Trillion KRW in 2025 | Oct 2025 | [Link](https://www.dailysecu.com/news/articleView.html?idxno=201211) |

---

**Language / 언어:**  
🇰🇷 [한국어](./README_KO.md) · 🇺🇸 [English](./README_EN.md) · 🇨🇳 [中文](./README_ZH.md) · 🇯🇵 [日本語](./README_JA.md)
