# 🔗 URL Shortener

A full-stack URL shortener built with **React**, **Tailwind CSS**, **Shadcn UI**, and **Supabase**. Create short, shareable links, generate QR codes for them, and track click analytics — all from a clean, modern dashboard.

**🚀 Live Demo:** [url-shortener-seven-liart.vercel.app](https://url-shortener-seven-liart.vercel.app/)

---

## ✨ Features

- 🔐 **Authentication** — Sign up and log in securely (powered by Supabase Auth)
- ✂️ **Custom short links** — Shorten any long URL, with optional custom aliases
- 📱 **QR code generation** — Every short link comes with an auto-generated, downloadable QR code
- 📊 **Click analytics** — Track clicks by device, location, and time with interactive charts
- 🎨 **Modern UI** — Responsive design built with Tailwind CSS and Shadcn UI components
- ⚡ **Fast** — Powered by Vite for instant dev feedback and optimized builds

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React, Vite |
| Styling | Tailwind CSS, Shadcn UI, Radix UI |
| Backend / DB | Supabase (Postgres, Auth, Storage) |
| Charts | Recharts |
| Forms & Validation | React Hook Form, Yup |
| Deployment | Vercel |

---

## 📦 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or later recommended)
- A free [Supabase](https://supabase.com/) account

### 1. Clone the repository

```bash
git clone https://github.com/<your-username>/url-shortener.git
cd url-shortener
```

### 2. Install dependencies

```bash
npm install
```

### 3. Set up Supabase

1. Create a new project at [supabase.com](https://supabase.com/).
2. In the SQL editor, create the required tables (`urls`, `clicks`) and a storage bucket (`qrs`) for QR codes.
3. Enable Row Level Security (RLS) and add policies so users can only manage their own links.
4. Grab your **Project URL** and **anon/public API key** from *Project Settings → API*.

### 4. Configure environment variables

Create a `.env` file in the project root:

```dotenv
VITE_SUPABASE_URL=your_supabase_project_url
VITE_SUPABASE_KEY=your_supabase_anon_key
```

### 5. Run the app

```bash
npm run dev
```

The app will be available at `http://localhost:5173`.

---

## 📁 Project Structure

```
url-shortener/
├── public/           # Static assets
├── src/
│   ├── components/   # Reusable UI components
│   ├── context/       # App-wide context (auth, etc.)
│   ├── db/            # Supabase queries and API helpers
│   ├── hooks/          # Custom React hooks
│   ├── pages/          # Route-level pages
│   └── main.jsx        # App entry point
├── .env               # Environment variables (not committed)
└── package.json
```

---

## 🚀 Deployment

This project is deployed on [Vercel](https://vercel.com/). To deploy your own copy:

1. Push your code to GitHub.
2. Import the repo into Vercel.
3. Add `VITE_SUPABASE_URL` and `VITE_SUPABASE_KEY` as environment variables in the Vercel project settings.
4. Deploy 🎉

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome. Feel free to open a pull request or issue.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

# 👩‍💻 Author

### Pragati 

Full Stack Developer 

- 💼 Open to Software Engineering Opportunities
- 🌎 India
- 💻 Passionate about Scalable Web Applications
- 🚀 Building Production-Ready SaaS Products

 ---

# ⭐ Show Your Support

If you found this project helpful,

⭐ Star this repository

🍴 Fork this repository

🐛 Report Issues

💡 Share Feedback

---

<div align="center">

### 🚀 Built with ❤️ using Next.js 15, TypeScript, Prisma & Supabase

**If you like this project, don't forget to leave a ⭐ on GitHub!**

</div>
