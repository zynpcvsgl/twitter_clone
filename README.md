# Fullstack X Twitter Clone: Next.js 13, React, TypeScript, Prisma, Clerk, Tailwind CSS, Cloudinary, MySQL, Shadcn UI, Zustand

This is a full-stack clone of Twitter built with **Next.js 13**, **React**, **TypeScript**, and several modern technologies such as **Prisma**, **Clerk**, **Tailwind CSS**, **Cloudinary**, and **MySQL**. It offers core features of Twitter, such as creating and deleting tweets, following users, notifications, and more.


## Key Features

- **Create Tweet** – Upload images, add links, and write text
- **Delete Tweet**
- **Share Tweet**
- **Reply to Tweet**
- **Like Tweet**
- **Bookmark Tweet**
- **Follow User**
- **Notifications** – Receive updates for likes, comments, replies, follows
- **Search Menu** – Find users by their username
- **Search & Explore Page** – Discover tweets and users
- **Edit Profile** – Manage personal details and image
- **Profile Page** – View posts, replies, and liked tweets
- **Pagination** – Navigate through large datasets
- **Beautiful UI** using **TailwindCSS** and **Shadcn UI**
- **Fully Responsive** – Optimized for mobile devices
- **MySQL Database** using Railway
- **ORM** with **Prisma**
- **Authentication** with **Clerk**

## Project Setup

To run this project locally, follow these steps:

1. Clone the Repository
    ```bash
    git clone https://github.com/zynpcvsgl/twitter_clone.git
    cd twitter_clone
    ```

2. Install Dependencies

    You can install the required packages using your preferred package manager:

    - **npm**:
        ```bash
        npm install
        ```

    - **yarn**:
        ```bash
        yarn install
        ```

    - **pnpm**:
        ```bash
        pnpm install
        ```

    - **bun**:
        ```bash
        bun install
        ```

3. Set up `.env` file

    Create a `.env` file in the root directory of the project and add the following environment variables:

    ```bash
    # CLERK
    NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_publishable_key
    CLERK_SECRET_KEY=your_secret_key
    NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
    NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
    NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
    NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding

    # DATABASE (Use MySQL URL from your Railway or other MySQL provider)
    DATABASE_URL=your_database_url

    # CLOUDINARY
    NEXT_PUBLIC_CLOUDINARY_NAME=your_cloudinary_name
    NEXT_PUBLIC_UPLOAD_PRESET=your_upload_preset

    # NEXT URL
    NEXT_PUBLIC_NEXT_URL=http://localhost:3000
    ```

4. Set up Prisma

    You need to generate Prisma's client and apply the migrations:

    ```bash
    npx prisma generate
    npx prisma db push
    ```

5. Running the App

    After completing the above setup, you can run the app in development mode:

    ```bash
    npm run dev
    ```

    This will start the server at `http://localhost:3000`.


