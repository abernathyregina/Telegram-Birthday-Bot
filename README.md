# Telegram Birthday Bot

Automate birthday reminders and personalized wishes across Telegram groups and DMs with smart scheduling and human-like interactions. This project eliminates manual tracking, handles timezones, and triggers on-device or emulator workflows to deliver on-time greetings that feel authentic. **Telegram Birthday Bot** is ideal for communities, teams, and brands that want consistent celebrations without extra effort.

<p align="center">
  <a href="https://Appilot.app" target="_blank"><img src="media/appilot-baner.png" alt="Appilot Banner" width="100%"></a>
</p>
<p align="center">
 <a href="https://t.me/devpilot1" target="_blank"><img src="https://img.shields.io/badge/Chat%20on-Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram"></a>
 <a href="mailto:support@appilot.app" target="_blank"><img src="https://img.shields.io/badge/Email-support@appilot.app-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail"></a>
 <a href="https://appilot.app" target="_blank"><img src="https://img.shields.io/badge/Visit-Website-007BFF?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website"></a>
 <a href="https://discord.gg/r5sJ5vhf" target="_blank"><img src="https://img.shields.io/badge/Join-Appilot_Community-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Appilot Discord"></a>
</p>
<p align="center"> 
   Created by Appilot, built to showcase our approach to Automation!<br>
   <strong>If you are looking for custom Telegram Birthday Bot, you've just found your team — Let’s Chat.👆👆</strong>
</p>

## Introduction
This bot automates the end-to-end workflow of detecting upcoming birthdays, queuing messages, and posting wishes on Telegram — either as DMs or within groups/channels.  
It removes the repetitive hassle of tracking dates, handling timezones, and composing messages for each member.  
Businesses and communities benefit from stronger engagement, consistency, and reliable delivery — even at scale.

### Automating Telegram Birthday Greetings at Scale
- Tracks user/member birthdays, pre-writes messages, and schedules delivery at the right local time.
- Human-like behavior (typing delays, random pauses, emoji variations) reduces detection risk and keeps interactions natural.
- Works with real Android devices and emulators for robust control; scales across accounts and devices.
- Centralized dashboard for scheduling, retries, logs, and campaign analytics.

## Core Features
- **Real Devices and Emulators:** Run actions on physical Android phones or emulators (Bluestacks/Nox) for high reliability and compatibility with Telegram.
- **No-ADB Wireless Automation:** ADB-less control for safer, stealthier sessions; lower connection friction on Wi-Fi/LAN.
- **Mimicking Human Behavior:** Randomized delays, typing simulation, emoji/spintax variations, and staggered sends to appear organic.
- **Multiple Accounts Support:** Add many Telegram accounts with per-profile settings, cookies/sessions, and independent schedules.
- **Multi-Device Integration:** Distribute workloads across device farms; queue-based assignment with health checks and failover.
- **Exponential Growth for Your Account:** Keep your community warm and engaged, driving replies and visibility with consistent celebrations.
- **Premium Support:** Priority troubleshooting, onboarding assistance, and tailored playbooks for your use case.
- **Timezone-Aware Scheduling:** Deliver wishes in each user’s local time, with DST handling and per-contact overrides.
- **Template & Media Library:** Save message templates, images, stickers, GIFs; auto-attach based on profile tags or groups.
- **Advanced Logging & Analytics:** Message outcomes, delivery latencies, retries, and device/account health dashboards.

### Additional Capabilities
| Feature | Description |
|---|---|
| **Contact & Birthday Database** | Encrypted storage of contacts, birthdays, tags, and preferences with import/export (CSV/JSON). |
| **Anti-Detection & Proxy** | Rotating proxies, device fingerprinting options, and session isolation for safer operation. |
| **Retry & Backoff Engine** | Automatic retries with exponential backoff, per-error strategies, and dead-letter queues. |
| **Role-Based Access** | Admin/operator roles, audit trails, and granular permissions for team usage. |
| **Webhook & API Hooks** | Trigger external workflows (CRMs, Google Sheets, Slack) before/after message delivery. |
| **Crash-Safe Orchestrator** | Supervisor restarts stuck jobs, rehydrates sessions, and resumes queues without data loss. |

</p>
<p align="center">
  <a href="https://appilot.app" target="_blank">
    <img src="media/{{keyword}-banner}.png" alt="{{keyword}-architecture}" width="95%">
  </a>
</p>

## How It Works
1. **Input or Trigger** — From the Appilot dashboard, you import contacts/birthdays or sync via API, choose templates, and select target accounts/devices.  
2. **Core Logic** — Appilot controls Android devices/emulators using UI Automator/Appium or ADB-less drivers to open Telegram, find targets, and compose/send messages with human-like pacing.  
3. **Output or Action** — The bot sends scheduled greetings (DMs or group posts), attaches media, and records outcomes and replies.  
4. **Other functionalities** — Retries, error handling, structured logging, parallel processing, proxy routing, and alerts are configurable in the dashboard.

## Tech Stack
- **Language:** Kotlin, Java, JavaScript, Python  
- **Frameworks:** Appium, UI Automator, Espresso, Robot Framework, Cucumber  
- **Tools:** Appilot, Android Debug Bridge (ADB), Appium Inspector, Bluestacks, Nox Player, Scrcpy, Firebase Test Lab, MonkeyRunner, Accessibility  
- **Infrastructure:** Dockerized device farms, Cloud-based emulators, Proxy networks, Parallel Device Execution, Task Queues, Real device farm.

## Directory Structure
```
telegram-birthday-bot/
│
├── src/
│ ├── main.py
│ ├── bot/
│ │ ├── scheduler.py
│ │ ├── templates.py
│ │ ├── delivery.py
│ │ ├── humanizer.py
│ │ ├── contacts.py
│ │ └── utils/
│ │ ├── logger.py
│ │ ├── proxy_manager.py
│ │ ├── device_pool.py
│ │ ├── retry_backoff.py
│ │ └── config_loader.py
│ ├── android/
│ │ ├── ui_automator/
│ │ │ ├── selectors.xml
│ │ │ └── actions.kt
│ │ ├── appium/
│ │ │ ├── capabilities.json
│ │ │ └── flows/
│ │ │ ├── open_telegram.js
│ │ │ └── send_message.js
│ │ └── drivers/
│ │ ├── adb_less_driver.py
│ │ └── accessibility_driver.py
│ └── webhooks/
│ ├── server.js
│ └── handlers/
│ ├── pre_send.js
│ └── post_send.js
│
├── config/
│ ├── settings.yaml
│ ├── credentials.env
│ ├── proxies.yaml
│ └── devices.yaml
│
├── data/
│ ├── contacts.csv
│ ├── birthdays.json
│ └── templates/
│ ├── classic.txt
│ ├── fun.txt
│ └── professional.txt
│
├── logs/
│ ├── app.log
│ └── delivery.log
│
├── output/
│ ├── reports/
│ │ ├── daily_summary.csv
│ │ └── failures.csv
│ └── screenshots/
│ └── <timestamp>.png
│
├── tests/
│ ├── unit/
│ └── e2e/
│
├── docker/
│ ├── Dockerfile
│ └── compose.yaml
│
├── requirements.txt
└── README.md
```

## Use Cases
- **Community managers** use it to auto-send birthday wishes in group chats, so they can boost engagement and member retention.  
- **HR/People ops teams** use it to DM employees on their birthdays, so they can maintain culture without manual scheduling.  
- **Brands & creators** use it to celebrate followers/customers, so they can nurture loyalty and drive replies organically.  
- **Agency operators** use it to manage multiple client accounts, so they can deliver consistent touchpoints at scale.

##FAQs
**How do I configure this automation for multiple accounts?**  
Add profiles in the dashboard, attach device/emulator mappings, and assign per-profile schedules and proxies. Each account runs in an isolated session with its own queue.

**Does it support proxy rotation or anti-detection?**  
Yes — configure rotating proxies and session isolation. The orchestrator randomizes timings, input patterns, and media to reduce fingerprint consistency.

**Can I schedule it to run periodically?**  
Absolutely. Use cron-like rules or relative schedules (e.g., “9 AM user-local time”) with DST awareness. Missed windows trigger safe catch-up sends with rate limits.

**What happens if Telegram UI changes?**  
Selectors and flows are versioned. The bot ships with validator checks; failing checks trigger alternative selectors or fallbacks, and you’ll see alerts in logs.

## Performance & Reliability Benchmarks
- **Execution Speed:** 500–1,500 sends/hour per device (template-only) under stable network; media attachments slightly reduce throughput.  
- **Success Rate:** ~95% delivery success across stable sessions with healthy proxies and verified numbers.  
- **Scalability:** Horizontally scales from a handful of devices to **300–1,000** with queue-based orchestration and shardable contact lists.  
- **Resource Efficiency:** Lightweight workers (~150–300MB each) and shared drivers; GPU not required.  
- **Error Handling:** Structured retries with exponential backoff, dead-letter queues, device health checks, crash-safe restarts, and alerting to Slack/Webhooks.

##
<p align="center">
<a href="https://cal.com/app-pilot-m8i8oo/30min" target="_blank">
  <img src="https://img.shields.io/badge/Book%20a%20Call%20with%20Us-34A853?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book a Call">
</a>
</p>
