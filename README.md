# Sports Dunia Dashboard

## Project Overview

The **Sports Dunia Dashboard** is a responsive web application that provides analytics, data export options, and payout management for articles and blogs. It includes a variety of features designed to enhance user experience and productivity.

---

## Features

### **Authentication**
- Login via email
- GitHub OAuth

### **Dashboard Modules**

1. **Overview**
   - Total number of articles/blogs fetched from an API
   - Payout analytics through interactive charts
   - Dynamic filtering and export to CSV/PDF

2. **Articles Section**
   - Article listing with filters (author, date, global search)
   - Displays payout per article/blog

3. **News Analysis**
   - Author trends displayed via pie/bar charts

4. **Payout Details**
   - Tabular breakdown of article payouts
   - Export capabilities

5. **Admin Only Features**
   - Access control based on user roles
   - Special admin dashboard section

---

## Tech Stack

- **Framework:** Next.js 14 (App Router)
- **Styling:** Tailwind CSS
- **Authentication:** NextAuth.js
- **State Management:** Context API or hooks

---

## Folder Structure

```
src/
├── app/                 # All route-based files (App Router)
│   ├── (auth)/          # Authentication pages
│   ├── dashboard/       # Main dashboard views
├── components/          # Reusable components
├── lib/                 # Utilities (API helpers, auth config)
├── styles/              # Global styles
public/                  # Static assets
```

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/SportsDunia-Dashboard.git
cd SportsDunia-Dashboard
```

### 2. Install Dependencies

Make sure you have **Node.js >= 18** installed.

```bash
npm install
```

### 3. Environment Variables

Create a `.env.local` file in the root directory and add the following:

```env
NEXTAUTH_SECRET=your_secret_here
NEXTAUTH_URL=http://localhost:3000
GITHUB_ID=your_github_oauth_id
GITHUB_SECRET=your_github_oauth_secret
API_URL=https://your-api-endpoint.com
```

> ⚠️ Get your GitHub credentials from [GitHub Developer Settings](https://github.com/settings/developers).

### 4. Run the App Locally

```bash
npm run dev
```

The app will run at: [http://localhost:3000](http://localhost:3000)

---

## Deployment

To deploy to Vercel:

1. Push your code to GitHub
2. Connect GitHub to [Vercel](https://vercel.com/)
3. Set environment variables in Vercel Dashboard
4. Deploy!

---

## Export Options

- Articles and payout tables can be exported as:
  - **CSV**
  - **PDF**
- Filters affect export output dynamically

---

## License

MIT

---

