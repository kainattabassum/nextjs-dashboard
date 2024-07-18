## Next.js App Router Course - Starter

This is the starter template for the Next.js App Router Course. It contains the starting code for the dashboard application.

For more information, see the [course curriculum](https://nextjs.org/learn) on the Next.js Website.

---
### Styling: 
The different ways to style your application in Next.js.
### Optimizations: 
How to optimize images, links, and fonts.
### Routing: 
How to create nested layouts and pages using file-system routing.
### Data Fetching: 
How to set up a database on Vercel, and best practices for fetching and streaming.
### Search and Pagination: 
How to implement search and pagination using URL Search Params.
### Mutating Data: 
How to mutate data using React Server Actions, and revalidate the Next.js cache.
### Error Handling: 
How to handle general and 404 not found errors.
### Form Validation and Accessibility: 
How to do server-side form validation and tips for improving accessibility.
### Authentication: 
How to add authentication to your application using NextAuth.js and Middleware.
## Metadata: 
How to add metadata and prepare your application for social sharing.

---
### Create new project 
    - npm install -g pnpm
    - npx create-next-app@latest nextjs-dashboard --example "https://github.com/vercel/next-learn/tree/main/dashboard/starter-example" --use-pnpm

### /app: 
Contains all the routes, components, and logic for your application, this is where you'll be mostly working from.

#### /app/lib: 
Contains functions used in your application, such as reusable utility functions and data fetching functions.

#### /app/ui: 
Contains all the UI components for your application, such as cards, tables, and forms. To save time, we've pre-styled these components for you.

### /public: 
Contains all the static assets for your application, such as images.
Config Files: You'll also notice config files such as next.config.js at the root of your application. Most of these files are created and pre-configured when you start a new project using create-next-app. You will not need to modify them in this course.

---

### Placeholder data
When you're building user interfaces, it helps to have some placeholder data. If a database or API is not yet available, you can:

- Use placeholder data in JSON format or as JavaScript objects.
- Use a 3rd party service like [Mock API](https://mockapi.io)

If you're a TypeScript developer:

We're manually declaring the data types, but for better type-safety, we recommend [Prisma](https://www.prisma.io) or [Drizzle](https://orm.drizzle.team), which automatically generates types based on your database schema.
Next.js detects if your project uses TypeScript and automatically installs the necessary packages and configuration. Next.js also comes with a TypeScript plugin for your code editor, to help with auto-completion and type-safety.

    Using the clsx library to toggle class names

---
### What is streaming?
Streaming is a data transfer technique that allows you to break down a route into smaller "chunks" and progressively stream them from the server to the client as they become ready.

There are two ways you implement streaming in Next.js:

    - At the page level, with the loading.tsx file.
    - For specific components, with <Suspense>.

--- 
### Partial Prerendering:
Partial Prerendering – a new rendering model that allows you to combine the benefits of static and dynamic rendering in the same route.