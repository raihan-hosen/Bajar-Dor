# 🛒 বাজার দর (Bazar Dor)

## 📖 Short Description
**Bazar Dor** is a modern, responsive web application built to help users track the daily market prices of essential commodities in Bangladesh. It features real-time price fluctuation tracking, categorized product browsing, secure user authentication, and detailed market-wise price summaries. 

🔗 **Live Link:** [Insert Live Link Here]
🔗 **GitHub Repository:** [Insert Repo Link Here]

---

## ✨ Key Features

1. **Live Price Ticker & Fluctuation Tracking:** An infinite scrolling marquee in the navbar displays current prices and percentage changes (▲/▼). The home page highlights the top 6 price risers ("আজ দাম বেড়েছে") and top 6 fallers ("আজ দাম কমেছে").
2. **Advanced Sorting with Bengali Numerals:** Users can sort category products by price (Default, Low to High, High to Low), with the sorting algorithm fully supporting Bengali numerical characters.
3. **Protected Product Details:** Authenticated users can view detailed insights for specific items, including minimum, maximum, and average prices, alongside a breakdown of prices across different local markets.
4. **Secure Authentication & Profile Management:** Seamless and secure Sign Up and Sign In flows using BetterAuth (supporting both Email/Password and Social Login). Users can also securely update their profile information.
5. **Robust UX & Responsive Design:** A fully responsive UI across all devices (Mobile, Tablet, Desktop) featuring loading skeletons for data fetching, interactive toast notifications for user actions, and a friendly, custom 404 error page.

---

## 🛠️ Technologies Used

* **Framework:** Next.js (App Router)
* **Language:** TypeScript / JavaScript
* **Styling:** Tailwind CSS (with DaisyUI / Hero UI)
* **Authentication:** BetterAuth
* **Notifications:** react-hot-toast / data-rht-toaster
* **Deployment:** Vercel / Netlify / Cloudflare Pages

---

## ⚙️ Getting Started Locally

To run this project on your local machine, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone <your-github-repo-link>
   cd bazar-dor
   ```

2. **Install dependencies:**
   ```bash
   npm install
   # or yarn install / pnpm install
   ```

3. **Set up Environment Variables:**
   Create a `.env.local` file in the root directory and add the necessary environment variables for BetterAuth and your API URLs:
   ```env
   NEXT_PUBLIC_API_URL=https://openapi.programming-hero.com/api/bazardor
   # Add BetterAuth secrets and NextAuth URLs here
   ```

4. **Run the development server:**
   ```bash
   npm run dev
   ```

5. **Open the app:**
   Navigate to [http://localhost:3000](http://localhost:3000) in your browser to see the result.

---

## 📡 API Endpoints Used

* **Base URL:** `https://openapi.programming-hero.com/api/bazardor` (or alternative workers)
* `GET /products` - Fetch all products
* `GET /products?category={category_name}` - Filter products by category
* `GET /products/{id}` - Fetch single product details
* `GET /categories` - Fetch all categories
* `GET /categories/{category_name}` - Fetch a single category