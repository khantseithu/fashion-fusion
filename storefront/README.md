# Fashion Fusion Storefront (Next.js 13, Tailwind, Prisma, MySQL, Clerk, Stripe)

Deployed on Vercel: [https://fashion-fusion-storefront.vercel.app/](https://fashion-fusion-storefront.vercel.app/)

For DEMO, use [Stripe Testing Cards](https://stripe.com/docs/testing)

This is a repository for a Full Stack E-Commerce + Dashboard & CMS: Next.js 13 App Router, React, Tailwind, Prisma, MySQL

Key Features:

- We will be using Shadcn UI for the Admin!
- Our admin dashboard is going to serve as both CMS, Admin and API!
- You will be able to control mulitple vendors / stores through this single CMS! (For example you can have a "Shoe store" and a "Laptop store" and a "Suit store", and our CMS will generate API routes for all of those individually!)
- You will be able to create, update and delete categories!
- You will be able to create, update and delete products!
- You will be able to upload multiple images for products, and change them whenever you want!
- You will be able to create, update and delete filters such as "Color" and "Size", and then match them in the "Product" creation form.
- You will be able to create, update and delete "Billboards" which are these big texts on top of the page. You will be able to attach them to a single category, or use them standalone (Our Admin generates API for all of those cases!)
- You will be able to Search through all categories, products, sizes, colors, billboards with included pagination!
- You will be able to control which products are "featured" so they show on the homepage!
- You will be able to see your orders, sales, etc.
- You will be able to see graphs of your revenue etc.
- You will learn Clerk Authentication!
- Order creation
- Stripe checkout
- Stripe webhooks
- MySQL + Prisma + PlanetScale

## Folder Structure

```bash
.
├── LICENSE
├── README.md
├── actions
│   ├── get-billboard.tsx
│   ├── get-categories.tsx
│   ├── get-category.tsx
│   ├── get-colors.tsx
│   ├── get-product.tsx
│   ├── get-products.tsx
│   └── get-sizes.tsx
├── app
│   ├── (routes)
│   │   ├── cart
│   │   │   ├── components
│   │   │   │   ├── cart-item-info.tsx
│   │   │   │   ├── cart-item.tsx
│   │   │   │   └── summary.tsx
│   │   │   └── page.tsx
│   │   ├── category
│   │   │   └── [categoryId]
│   │   │       ├── components
│   │   │       │   ├── filter.tsx
│   │   │       │   └── mobile-filters.tsx
│   │   │       ├── loading.tsx
│   │   │       └── page.tsx
│   │   ├── loading.tsx
│   │   ├── page.tsx
│   │   └── product
│   │       └── [productId]
│   │           ├── loading.tsx
│   │           └── page.tsx
│   ├── favicon.ico
│   ├── globals.css
│   └── layout.tsx
├── components
│   ├── footer.tsx
│   ├── gallery
│   │   ├── gallery-tab.tsx
│   │   └── index.tsx
│   ├── info.tsx
│   ├── main-nav.tsx
│   ├── navbar-actions.tsx
│   ├── navbar.tsx
│   ├── preview-modal.tsx
│   ├── product-list.tsx
│   └── ui
│       ├── billboard.tsx
│       ├── button.tsx
│       ├── container.tsx
│       ├── currency.tsx
│       ├── icon-button.tsx
│       ├── modal.tsx
│       ├── no-results.tsx
│       ├── product-card.tsx
│       └── skeleton.tsx
├── constants.ts
├── hooks
│   ├── use-cart.tsx
│   └── use-preview-modal.ts
├── lib
│   └── utils.ts
├── next.config.js
├── package-lock.json
├── package.json
├── postcss.config.js
├── providers
│   ├── modal-provider.tsx
│   └── toast-provider.tsx
├── public
│   ├── bag.png
│   ├── bg.svg
│   ├── billboard-bg-2.png
│   ├── billboard-bg-3.png
│   ├── billboard-bg.png
│   ├── coat.png
│   ├── image.png
│   ├── next.svg
│   ├── scarf.png
│   ├── user.png
│   └── vercel.svg
├── tailwind.config.js
├── tsconfig.json
└── types.ts

17 directories, 66 files
```
