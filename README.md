# SandClaw

### *Raise your own AI trader from scratch.*

**AI-Powered Trading Desktop IDE** &nbsp; ![beta](https://img.shields.io/badge/v0.9.1-beta-orange)

> **Beta Release** = Some features may have bugs. Please report issues via [GitHub Issues](https://github.com/kokogo100/sandclaw-releases/issues).

### Important Notice

- **Free to use.** No deposits, no withdrawals, no fees.
- **Your funds stay with your broker.** SandClaw connects directly to broker APIs via plugins. We never hold or access your money.
- **No investment advice.** SandClaw does not provide investment recommendations or financial advice. It is delivered as a complete blank slate, adapting to your own analysis and judgment.
- **AI starts from zero.** The AI has no preloaded opinions. It learns from your conversations and builds memory over time.
- **Open plugin ecosystem.** Connect to 30+ brokers (LS Securities, IBKR, Kraken, Upbit, etc.) through installable plugins.
- **Community-driven plugins.** Request a broker plugin via [GitHub Issues](https://github.com/kokogo100/sandclaw-releases/issues). When enough users request it, we build it.
- **No built-in charts.** SandClaw is designed to work alongside your broker. Use your broker's charts and tools for technical analysis. SandClaw handles AI strategy, automation, and execution.

---

> [!CAUTION]
> **v0.9.0 Users — Manual Update Required**
>
> v0.9.0 had a JWT key renewal issue. We released v0.9.1 to fix it, but discovered that **auto-update does not work from v0.9.0**.
> v0.9.0 users must manually download and install v0.9.1 by overwriting the existing installation for future updates to work.
>
> ⛔ **Do NOT fully uninstall SandClaw — this will permanently delete your L4 Memory Keys. Always install by overwriting (run the installer without uninstalling first).**

---

## Download

| Version | Windows (x64) | macOS | Release Notes |
|---------|--------------|-------|---------------|
| v0.9.1-beta | [SandClaw_0.9.1_x64-setup.exe](https://github.com/kokogo100/sandclaw-releases/releases/download/v0.9.1/SandClaw_0.9.1_x64-setup.exe) | Coming soon | [Release Notes](https://github.com/kokogo100/sandclaw-releases/releases/tag/v0.9.1) |

> macOS version will be added when there is sufficient user demand. Request via [GitHub Issues](https://github.com/kokogo100/sandclaw-releases/issues).

---

### ⚠️ Windows SmartScreen Notice

When you run the installer for the first time, Windows may show a **blue or red SmartScreen warning**.
This is normal for new applications without a paid code signing certificate (~$300/year).

1. Click **"More info"** (추가 정보)
2. Click **"Run anyway"** (실행)

> SandClaw is open source. You can verify the code at [GitHub](https://github.com/kokogo100/sandclaw).

---

## Installation

1. **Download** the installer above
2. **Run** `SandClaw_0.9.1_x64-setup.exe` and follow the setup wizard
3. **Python Setup** = the app automatically installs the Python environment on first launch
4. **Login** = sign in with GitHub or Discord

---

## UI Guide

### Main View

![Main View](images/Main%20View.png)

<details>
<summary><strong>1. Strategy List</strong></summary>
List of active strategies. Select the strategy to run using the radio button.
</details>

<details>
<summary><strong>2. Layout Buttons</strong></summary>
Switch the screen layout. Supports 4 modes: Grid, Horizontal Split, Vertical Split, and Fullscreen.
</details>

<details>
<summary><strong>3. Sidebar Navigation</strong></summary>
Left icon menu. Arranged in order: Strategy, Prompt, Settings, Account, Help.
</details>

<details>
<summary><strong>4. New Strategy</strong></summary>
Button to create a new trading strategy.
</details>

<details>
<summary><strong>5. My Account</strong></summary>
Displays the current account total assets, invested amount, P&L, and cash balance.
</details>

<details>
<summary><strong>6. Current Holdings</strong></summary>
Holdings table showing ticker, name, price, average cost, quantity, invested amount, market value, P&L, and sell button.
</details>

<details>
<summary><strong>7. Groups (Left)</strong></summary>
Watchlist group list. Create multiple groups to categorize your stocks.
</details>

<details>
<summary><strong>8. Groups (Right)</strong></summary>
Quotes for the selected group. Shows ticker, current price, change %, and volume.
</details>

<details>
<summary><strong>9. Context Files</strong></summary>
AI analysis priority notes. Checked files are automatically injected into the AI prompt.
</details>

<details>
<summary><strong>10. Plugin Tabs</strong></summary>
Bottom tabs to view account info and holdings for installed plugins.
</details>

<details>
<summary><strong>11. Chat Area</strong></summary>
AI chatbot conversation area. Ask market questions, search news, place orders using natural language.
</details>

<details>
<summary><strong>12. System Logs</strong></summary>
System log panel. Supports ALL/TRADE/AI/SYSTEM filters and INFO/WARN/ERROR/DEBUG level filters. Also includes Terminal and Engine tabs.
</details>

<details>
<summary><strong>13. Strategy Name</strong></summary>
The currently selected strategy name is displayed at the top.
</details>

<details>
<summary><strong>14. AI Manager</strong></summary>
AI Manager button. Manage AI Provider selection, prompt configuration, and MCP server connections.
</details>

<details>
<summary><strong>15. Settings</strong></summary>
Settings button. Manage all settings including trading, stop loss, alerts, watchlist, schedule, and system.
</details>

<details>
<summary><strong>16. Plugin & Skill Store</strong></summary>
Plugin and Skill Store button. Install/manage broker plugins and search/install AI skills.
</details>

<details>
<summary><strong>17. API Mode</strong></summary>
Indicates REST API mode or WebSocket mode based on the broker connection method.
</details>

---

### Settings

![Settings](images/Settings.png)

<details>
<summary><strong>1. Trading Tab</strong></summary>
Configure order type (market/limit), buy/sell ratio, and duplicate purchase prevention.
</details>

<details>
<summary><strong>2. Stop Loss Tab</strong></summary>
Set stop loss ratio, trailing stop, and take profit ratio.
</details>

<details>
<summary><strong>3. Alerts Tab</strong></summary>
Configure PC sounds and external notifications (Telegram, Discord, etc.).
</details>

<details>
<summary><strong>4. Watchlist Tab</strong></summary>
Watchlist management. Create/delete groups and add/remove stocks.
</details>

<details>
<summary><strong>5. Schedule Tab</strong></summary>
Set engine auto start/stop times.
</details>

<details>
<summary><strong>6. Autopilot Tab</strong></summary>
Configure investment style, paper trading graduation criteria, and 6 guardrails (max order size, daily trades, loss limit, drawdown limit, API budget, cooldown).
</details>

<details>
<summary><strong>7. System Tab</strong></summary>
Monitor system resources (CPU, Memory, Disk) in real time. Database schema management and backup features.
</details>

---

### AI Manager

![AI Manager](images/AI%20Manager.png)

<details>
<summary><strong>1. Configuration</strong></summary>
Toggle AI Co-Pilot ON/OFF, select AI Provider (Claude/GPT/Gemini), enter API key, and choose model.
</details>

<details>
<summary><strong>2. Web Search</strong></summary>
Set search engine priority (DuckDuckGo, Tavily).
</details>

<details>
<summary><strong>3. MCP Servers</strong></summary>
Add and manage external tools like Sequential Thinking, Filesystem, Memory Service, etc.
</details>

<details>
<summary><strong>4. Knowledge Links</strong></summary>
Inject reference website links to AI for news, finance, research, etc.
</details>

<details>
<summary><strong>5. Buy/Sell Prompts</strong></summary>
Save and select trading decision prompts for auto-trading.
</details>

---

### AI Commander

![AI Commander](images/AI%20Commander.png)

<details>
<summary><strong>1. Automation</strong></summary>
Detailed auto-trading settings. Manage Trading Mode, Safety Intercept, Daily Trading Limit.
</details>

<details>
<summary><strong>2. MCP Servers</strong></summary>
Manage real-time data sources.
</details>

<details>
<summary><strong>3. AI Hive</strong></summary>
AI Hive community settings. Configure autonomous community participation.
</details>

<details>
<summary><strong>4. Notifications</strong></summary>
Manage trade alerts and system notifications.
</details>

<details>
<summary><strong>5. Learning</strong></summary>
Configure the interval at which AI autonomously organizes memory and generates insights.
</details>

---

### Start Engine

![Start Engine](images/Start%20Engine.png)

<details>
<summary><strong>1. Trading Settings</strong></summary>
Review trading amount, max buy count, stop loss/take profit, trailing stop, and max holdings.
</details>

<details>
<summary><strong>2. Strategy Summary</strong></summary>
Displays applied filter count, custom conditions, margin trading, and alert settings.
</details>

<details>
<summary><strong>3. Smart Filter</strong></summary>
Technical indicator-based smart filter. Combine RSI, MACD, Bollinger Bands, and more.
</details>

<details>
<summary><strong>4. Chart Filter</strong></summary>
Chart pattern-based filter. Candle patterns, trend lines, and more.
</details>

<details>
<summary><strong>5. Custom Logic Filter</strong></summary>
User-defined condition filter. Single (1 condition), Expert (2), or Complex (3).
</details>

<details>
<summary><strong>6. AI ON/OFF & RESCAN</strong></summary>
Toggle AI analysis ON/OFF and set the rescan interval (15 min ~ 3 hours).
</details>

---

### Plugin Store

![Plugin Store](images/Plugin%20Store.png)

<details>
<summary><strong>1. Official Store / My Plugins</strong></summary>
Switch between Official Store and My Plugins tabs. Filter by API/Skills.
</details>

<details>
<summary><strong>2. Plugin List</strong></summary>
List of installable plugins. Status shown as INSTALLED/AVAILABLE badges.
</details>

<details>
<summary><strong>3. Plugin Detail</strong></summary>
Version, region, features, and description for the selected plugin.
</details>

<details>
<summary><strong>4. How It Works</strong></summary>
Step-by-step guide on how to use the plugin.
</details>

<details>
<summary><strong>5. Credential Vault</strong></summary>
Securely stores API keys with encryption in the credential vault.
</details>

---

## Key Features

| Feature | Description |
|---------|-------------|
| AI Chatbot | Claude, GPT, Gemini + Local LLM support |
| Auto Trading | Strategy-based automated trading engine |
| Autopilot (Paper) | Simulated trading to validate AI strategy |
| Autopilot (Live) | Fully autonomous AI trading after graduation |
| Plugin System | Connect brokers via 30+ plugins |
| Browser Agent | Web search, crawling, CDP automation |
| Memory System | Multi-tier memory architecture |
| Market Data | US, UK, JP, KR, Crypto daily snapshots |

---

## Links

- [Plugin Registry](https://github.com/kokogo100/sandclaw), 30+ broker plugins
- [Community & News](https://algoballoon.com)
- [MCP Server & API](https://ragalgo.com)

---

*SandClaw — AI Agent IDE. Free within fences.*
