# PostgreSQL SSH Dashboard

A modern, secure web-based dashboard for managing **PostgreSQL** databases on remote servers through an **SSH tunnel**.

![Dashboard Preview](public/previews/preview.png)

## ✨ Features

- **Secure SSH Tunneling** — Connect to PostgreSQL servers that are not directly accessible (behind firewalls, private networks, VPS, etc.)
- **SSH Authentication** — Support for password and private key authentication
- **PostgreSQL Administration**:
  - Browse databases
  - View tables and their structure
  - Preview table content (up to 150 rows)
  - Create and delete databases
  - Create, modify, and delete tables and columns
  - Manage PostgreSQL users (including Superuser role)
- **Modern UI** — Built with React 19, Tailwind CSS, and smooth animations
- **AI Assistant** — Integrated with Google Gemini (optional)
- **Multi-language support** — English, Russian, and more

## 🛠  Tech Stack

**Frontend:**
- React 19 + TypeScript
- Vite
- Tailwind CSS
- Lucide Icons
- Framer Motion

**Backend:**
- Node.js + Express
- `ssh2` — SSH tunneling
- `pg` — PostgreSQL client
- TypeScript

## 🚀 Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/DuneonDev/PostgreSQL-SSH-Dashboard.git
cd PostgreSQL-SSH-Dashboard
```

### 2. Install dependencies
```bash
npm install
```

### 3. Configure environment
```bash
cp .env.example .env
```
Edit `.env` and add your **Gemini API key** (optional):
```env
GEMINI_API_KEY=your_gemini_api_key_here
```

### 4. Run the application
**Development mode:**
```bash
npm run dev
```
**Production build:**
```bash
npm run build
npm start
```
The application will be available at `http://localhost:3000`

## 📸 Screenshots
![Dashboard Preview](public/screenshot/Screenshot-01.png)
![Dashboard Preview](public/screenshot/Screenshot-02.png)
![Dashboard Preview](public/screenshot/Screenshot-03.png)
![Dashboard Preview](public/screenshot/Screenshot-04.png)
![Dashboard Preview](public/screenshot/Screenshot-05.png)
![Dashboard Preview](public/screenshot/Screenshot-06.png)
![Dashboard Preview](public/screenshot/Screenshot-07.png)
![Dashboard Preview](public/screenshot/Screenshot-08.png)

## 🔒 Security Notes
- All PostgreSQL connections are established through SSH tunnels
- No direct exposure of PostgreSQL port (5432) to the internet
- Credentials are not stored — entered per session
- Use strong SSH keys in production

## 🧩 Project Structure
```text
├── src/                 # React frontend
├── server/              # Backend logic
├── server.ts            # Main server entry point
├── public/              # Static assets
├── .env.example         # Environment variables template
└── package.json
```

## 🤝 Contributing
Contributions are welcome! Feel free to open issues or submit pull requests.

---

## 📄 Licensing and Usage Notice
This project is released under the **MIT License**. However, please note the following important restrictions regarding branding and intellectual property:

* **Trademarks and Copyright:** The **"duneon"** name and all associated logos are **not** covered by the MIT License. They are protected by copyright and remain the exclusive property of the creator, **duneon**.

* **Permissions:** You are free to use, study, and modify the source code for your own purposes, as permitted by the MIT License.

* **Commercial Use and Distribution:** You may use the software for commercial projects or distribute it, provided that you strictly adhere to the terms of the MIT License. 

* **Branding Requirements:** If you choose to redistribute or create a derivative work for commercial purposes, you **must remove or change all "duneon" logos and references to the "duneon" name** within your version of the product.

*For the full text of the MIT License, please refer to the `LICENSE` file included in this repository.*

---

Made with ❤️ by Duneon — High-performance system solutions.
<br>
website: [duneon.dev](https://duneon.dev)
<br>
support: [support@duneon.dev](mailto:support+postgresqlsshdashboard@duneon.dev)

