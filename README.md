# A&B Fashion Production — React Storefront

A responsive clothing storefront built with React + Vite. Includes:
- Responsive home page, category filters, product search and sorting
- Product detail modal with size selection
- Interactive shopping bag with quantity controls
- Order details form that prepares a WhatsApp message
- Wholesale / factory inquiry section and contact form
- Newsletter demo, saved products, responsive mobile navigation

## Run locally

1. Install Node.js LTS from https://nodejs.org/ if it is not installed.
2. Extract this ZIP.
3. Open the extracted `ab_fashion_store` folder in VS Code.
4. Open Terminal in VS Code and run:

   ```bash
   npm install
   npm run dev
   ```

5. Open the local URL Vite prints (usually `http://localhost:5173`).

## Before publishing

Update the sample products, prices, product images, business location, contact details and delivery terms in `src/main.jsx`. Product photography currently uses Unsplash URLs and needs an internet connection.

### WhatsApp orders
The current version opens WhatsApp with a prepared message using `https://wa.me/?text=...`. To send directly to your business WhatsApp, replace the `wa.me/?text=` URL in both order/contact handlers with `wa.me/YOUR_COUNTRY_CODE_AND_NUMBER?text=`. Use digits only, including country code, without `+`, spaces or dashes. Test the number before launch.

### Important limitations
This is a full front-end storefront prototype, not a production commerce backend. The cart lives in browser memory and resets on refresh. Orders are not saved in a database, stock is not synchronized, and newsletter signup is only a demo. Cash on delivery and delivery coverage must be confirmed with your business. For real multi-user sales, add a backend/database and an order-management workflow.

## Free deployment with Vercel

1. Create a GitHub repository and upload the extracted project.
2. Sign in to https://vercel.com/ with GitHub and import the repository.
3. Framework preset: Vite. Build command: `npm run build`. Output directory: `dist`.
4. Deploy. Vercel will provide a public URL.

You can also use Netlify: import the GitHub repository, build command `npm run build`, publish directory `dist`.
