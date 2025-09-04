<div align="center" width="100%">
    <img src="./saasfly-logo.svg" width="128" alt="" />
</div>

# Saasfly </br>

<a href="https://trendshift.io/repositories/8929" target="_blank"><img src="https://trendshift.io/api/badge/repositories/8929" alt="saasfly%2Fsaasfly | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>

[![GitHub Actions Workflow Status][check-workflow-badge]][check-workflow-badge-link] [![GitHub License][github-license-badge]][github-license-badge-link] [![Discord][discord-badge]][discord-badge-link] [![Saasfly][made-by-nextify-badge]][made-by-nextify-badge-link]
[![Chinese](https://img.shields.io/badge/-Chinese-red.svg)](README_zh.md)
[![German](https://img.shields.io/badge/-German-yellow.svg)](README_de.md)
[![Vietnamese](https://img.shields.io/badge/-Vietnamese-yellow.svg)](README_vi.md) </br>
![COMMIT_ACTIVITY](https://img.shields.io/github/commit-activity/m/saasfly/saasfly?style=for-the-badge">)
[![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fsaasfly%2Fsaasfly&labelColor=%23f47373&countColor=%23263759)](https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fsaasfly%2Fsaasfly)

An easy-to-use and enterprise-grade Next.js boilerplate.

You don't need to buy templates anymore; Saasfly provides a complete, open-source solution for building SaaS applications quickly and easily.

> **[Nextify](https://nextify.ltd)** provides a complete Enterprise SaaS solution. Contact us at [contact@nextify.ltd](mailto:contact@nextify.ltd) if you're interested in discussing your project, or if you'd simply like to have a conversation with us, please feel free to reach out.

> ❤️ We provide **free technical support and deployment services to non-profit organizations**.
>
> 🙌 All profits obtained from our open source projects will be **entirely dedicated to supporting open source initiatives and charitable causes**.

## ⚡ Live Demo

Try it out for yourself!

Demo Server (Location: Washington - USA): <https://show.saasfly.io>

See more documentation at <https://document.saasfly.io>

## 🌟 Star History

[![Star History Chart](https://app.repohistory.com/api/svg?repo=saasfly/saasfly&type=Timeline)](https://repohistory.com)

## Sponsors

<table>
  <tr>
   <td style="width: 64px;">
      <a href="https://libra.dev/">
        <div style="width: 64px;">
          <img alt="Clerk" src="https://raw.githubusercontent.com/nextify-limited/libra/main/logo.svg">
        </div>
      </a>
    </td>
    <td style="width: 64px;">
      <a href="https://go.clerk.com/uKDp7Au">
        <div style="width: 64px;">
          <img alt="Clerk" src="/clerk.png">
        </div>
      </a>
    </td>
    <td style="width: 64px;">
      <a href="https://www.twillot.com/">
        <div style="width: 64px;">
          <img alt="Take Control of All Your Twitter Assets" src="/twillot.png">
        </div>
      </a>
    </td>
    <td style="width: 64px;">
      <a href="https://www.setupyourpay.com/" title="如何注册美国公司进行收款">
        <div style="width: 64px;">
          <img alt="全球收款手册" src="/setupyourpay.png">
        </div>
      </a>
    </td>
  </tr>
</table>

<a href="mailto:contact@nextify.ltd">
  Add your logo here
</a>

## 🚀 Getting Started

### 🖱 One Click Template

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fsaasfly%2Fsaasfly&env=NEXT_PUBLIC_APP_URL,NEXTAUTH_URL,NEXTAUTH_SECRET,STRIPE_API_KEY,STRIPE_WEBHOOK_SECRET,POSTGRES_URL,GITHUB_CLIENT_ID,GITHUB_CLIENT_SECRET,RESEND_API_KEY,RESEND_FROM&install-command=bun%20install&build-command=bun%20run%20build&root-directory=apps%2Fnextjs)

### 📋 Prerequisites

Before you start, make sure you have the following installed:

1. [Bun](https://bun.sh/) & [Node.js](https://nodejs.org/) & [Git](https://git-scm.com/)

   1. Linux

   ```bash
     curl -sL https://gist.github.com/tianzx/874662fb204d32390bc2f2e9e4d2df0a/raw -o ~/downloaded_script.sh && chmod +x ~/downloaded_script.sh && source ~/downloaded_script.sh
   ```

   2. MacOS

   ```bash
     /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
     brew install git
     brew install oven-sh/bun/bun
     brew install nvm
   ```

2. [PostgreSQL](https://www.postgresql.org/)
   1. You can use Vercel Postgres or a local PostgreSQL server(add POSTGRES_URL env in .env.local)
      ```bash
         POSTGRES_URL = ''
      ```

### Installation

To get started with this boilerplate, we offer two options:

1. Use the `bun create` command(🌟Strongly recommend🌟):

```bash
bun create saasfly
```

2. Manually clone the repository:

```bash
git clone https://github.com/saasfly/saasfly.git
cd saasfly
bun install
```

### Setup

Follow these steps to set up your project:

1. Set up the environment variables:

```bash
cp .env.example .env.local
// (you must have a database prepared before running this command)
bun db:push
```

2. Run the development server:

```bash
bun run dev:web
```

3. Open [http://localhost:3000](http://localhost:3000) in your browser to see the result.

4. (Optional alpha)`bun run tailwind-config-viewer` Open [http://localhost:3333](http://localhost:3333) in your browser to see your Tailwind CSS configuration

### Other Notes

We are using Clerk as the default authentication provider after 1st June 2025.

You can find the NextAuth implementation here ( https://github.com/saasfly/saasfly/tree/feature-nextauth ) .

## 🥺 Project Roadmap

1. Admin Dashboard Page (in alpha !!!)
   1. Only provide static page now and we plan to integrate with headless arch
   2. You can provide your admin account and change **ADMIN_EMAIL="admin@saasfly.io,root@saasfly.io"** in .env.local and access host:port/admin/dashboard
   3. Based on security concerns, we will not provide online demos for the time being.
2. Consider integrating Payload CMS.

## ⭐ Features

### 🐭 Frameworks

- **[Next.js](https://nextjs.org/)** - The React Framework for the Web (with **App Directory**)
- **[NextAuth.js](https://next-auth.js.org/)** - Authentication for Next.js
- **[Kysely](https://kysely.dev/)** - The type-safe SQL query builder for TypeScript
- **[Prisma](https://www.prisma.io/)** - Next-generation ORM for Node.js and TypeScript, used as a schema management tool
- **[React-email](https://react.email/)** - A React renderer for creating beautiful emails using React components

### 🐮 Platforms

- **[Clerk](https://go.clerk.com/uKDp7Au)** - The most comprehensive User Management Platform
- **[Vercel](https://vercel.com/)** – Deploy your Next.js app with ease
- **[Stripe](https://stripe.com/)** – Payment processing for internet businesses
- **[Resend](https://resend.com/)** – Email marketing platform for developers

### 🐯 Enterprise Features

- **[i18n](https://nextjs.org/docs/app/building-your-application/routing/internationalization)** - Support for internationalization
- **[SEO](https://nextjs.org/docs/app/building-your-application/optimizing/metadata)** - Search engine optimization
- **[MonoRepo](https://turbo.build/)** - Monorepo for better code management
- **[T3 Env](https://env.t3.gg/)** - Manage your environment variables with ease

### 🐰 Data Fetching

- **[trpc](https://trpc.io/)** – End-to-end typesafe APIs made easy
- **[tanstack/react-query](https://react-query.tanstack.com/)** – Hooks for fetching, caching and updating asynchronous data in React

### 🐲 Global State Management

- **[Zustand](https://zustand.surge.sh/)** – Small, fast and scalable state management for React

### 🐒 UI

- **[Tailwind CSS](https://tailwindcss.com/)** – Utility-first CSS framework for rapid UI development
- **[Shadcn/ui](https://ui.shadcn.com/)** – Re-usable components built using Radix UI and Tailwind CSS
- **[Framer Motion](https://framer.com/motion)** – Motion library for React to animate components with ease
- **[Lucide](https://lucide.dev/)** – Beautifully simple, pixel-perfect icons
- **[next/font](https://nextjs.org/docs/basic-features/font-optimization)** – Optimize custom fonts and remove external network requests for improved performance

### 🐴 Code Quality

- **[TypeScript](https://www.typescriptlang.org/)** – Static type checker for end-to-end type safety
- **[Prettier](https://prettier.io/)** – Opinionated code formatter for consistent code style
- **[ESLint](https://eslint.org/)** – Pluggable linter for Next.js and TypeScript
- **[Husky](https://typicode.github.io/husky)** – Git hooks made easy

### 🐑 Performance

- **[Vercel Analytics](https://vercel.com/analytics)** – Real-time performance metrics for your Next.js app
- **[bun.sh](https://bun.sh/)** – npm alternative for faster and more reliable package management

### 🐘 Database

- **[PostgreSQL](https://www.postgresql.org/)** – The world's most advanced open source database

## 📦 Apps and Packages

- `web`: The main Next.js application
- `ui`: Shared UI components
- `db`: Database schema and utilities
- `auth`: Authentication utilities
- `email`: Email templates and utilities

## 📜 License

This project is licensed under the MIT License. For more information, see the [LICENSE](./LICENSE) file.

## 🙏 Credits

This project was inspired by shadcn's [Taxonomy](https://github.com/shadcn-ui/taxonomy) and t3-oss's [create-t3-turbo](https://github.com/t3-oss/create-t3-turbo).

## 👨‍💻 Contributors

<a href="https://github.com/saasfly/saasfly/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=saasfly/saasfly" />
</a>

Made with [contrib.rocks](https://contrib.rocks).

<!-- Badges and links -->

[check-workflow-badge]: https://img.shields.io/github/actions/workflow/status/saasfly/saasfly/ci.yml?label=ci
[github-license-badge]: https://img.shields.io/badge/License-MIT-green.svg
[discord-badge]: https://img.shields.io/discord/1204690198382911488?color=7b8dcd&link=https%3A%2F%2Fsaasfly.io%2Fdiscord
[made-by-nextify-badge]: https://img.shields.io/badge/made_by-nextify-blue?color=FF782B&link=https://nextify.ltd/
[check-workflow-badge-link]: https://github.com/saasfly/saasfly/actions/workflows/check.yml
[github-license-badge-link]: https://github.com/saasfly/saasfly/blob/main/LICENSE
[discord-badge-link]: https://discord.gg/8SwSX43wnD
[made-by-nextify-badge-link]: https://nextify.ltd

## 📁 Project Structure

```
saasfly
├─ apps
│  ├─ auth-proxy
│  │  ├─ package.json
│  │  ├─ routes
│  │  │  └─ [...auth].ts
│  │  └─ tsconfig.json
│  └─ nextjs
│     ├─ .contentlayer
│     │  ├─ .cache
│     │  │  └─ v0.4.3
│     │  │     ├─ compiled-contentlayer-config-SJYTHAIC.mjs
│     │  │     ├─ compiled-contentlayer-config-SJYTHAIC.mjs.map
│     │  │     └─ data-SJYTHAIC.json
│     │  ├─ generated
│     │  │  ├─ Author
│     │  │  │  ├─ authors__nok8s.mdx.json
│     │  │  │  ├─ _index.json
│     │  │  │  └─ _index.mjs
│     │  │  ├─ Doc
│     │  │  │  ├─ docs__documentation__index.mdx.json
│     │  │  │  ├─ docs__in-progress.mdx.json
│     │  │  │  ├─ docs__index.mdx.json
│     │  │  │  ├─ _index.json
│     │  │  │  └─ _index.mjs
│     │  │  ├─ Guide
│     │  │  │  ├─ guides__using-next-auth-next-14.mdx.json
│     │  │  │  ├─ _index.json
│     │  │  │  └─ _index.mjs
│     │  │  ├─ index.d.ts
│     │  │  ├─ index.mjs
│     │  │  ├─ Page
│     │  │  │  ├─ _index.json
│     │  │  │  └─ _index.mjs
│     │  │  ├─ Post
│     │  │  │  ├─ blog__deploying-next-apps.mdx.json
│     │  │  │  ├─ blog__dynamic-routing-static-regeneration.mdx.json
│     │  │  │  ├─ blog__preview-mode-headless-cms.mdx.json
│     │  │  │  ├─ blog__server-client-components.mdx.json
│     │  │  │  ├─ _index.json
│     │  │  │  └─ _index.mjs
│     │  │  └─ types.d.ts
│     │  └─ package.json
│     ├─ .eslintignore
│     ├─ .prettierignore
│     ├─ contentlayer.config.ts
│     ├─ next.config.mjs
│     ├─ package.json
│     ├─ postcss.config.cjs
│     ├─ public
│     │  ├─ favicon.ico
│     │  ├─ images
│     │  │  ├─ avatars
│     │  │  │  ├─ nok8s.jpeg
│     │  │  │  └─ saasfly-logo.svg
│     │  │  ├─ blog
│     │  │  │  ├─ blog-post-1.jpg
│     │  │  │  ├─ blog-post-2.jpg
│     │  │  │  ├─ blog-post-3.jpg
│     │  │  │  └─ blog-post-4.jpg
│     │  │  ├─ clerk.png
│     │  │  └─ noise.webp
│     │  ├─ logo.png
│     │  └─ logo.svg
│     ├─ src
│     │  ├─ app
│     │  │  ├─ admin
│     │  │  │  ├─ (dashboard)
│     │  │  │  │  └─ dashboard
│     │  │  │  │     ├─ layout.tsx
│     │  │  │  │     ├─ loading.tsx
│     │  │  │  │     └─ page.tsx
│     │  │  │  ├─ layout.tsx
│     │  │  │  └─ login
│     │  │  │     └─ page.tsx
│     │  │  ├─ api
│     │  │  │  ├─ auth
│     │  │  │  │  └─ [...nextauth]
│     │  │  │  │     └─ route.ts
│     │  │  │  ├─ trpc
│     │  │  │  │  └─ edge
│     │  │  │  │     └─ [trpc]
│     │  │  │  │        └─ route.ts
│     │  │  │  └─ webhooks
│     │  │  │     └─ stripe
│     │  │  │        └─ route.ts
│     │  │  ├─ layout.tsx
│     │  │  ├─ robots.ts
│     │  │  └─ [lang]
│     │  │     ├─ (auth)
│     │  │     │  ├─ layout.tsx
│     │  │     │  ├─ login
│     │  │     │  │  └─ page.tsx
│     │  │     │  ├─ login-clerk
│     │  │     │  │  └─ [[...rest]]
│     │  │     │  │     └─ page.tsx
│     │  │     │  └─ register
│     │  │     │     └─ page.tsx
│     │  │     ├─ (dashboard)
│     │  │     │  └─ dashboard
│     │  │     │     ├─ billing
│     │  │     │     │  ├─ loading.tsx
│     │  │     │     │  ├─ page.tsx
│     │  │     │     │  └─ subscription-form.tsx
│     │  │     │     ├─ layout.tsx
│     │  │     │     ├─ loading.tsx
│     │  │     │     ├─ page.tsx
│     │  │     │     └─ settings
│     │  │     │        ├─ loading.tsx
│     │  │     │        └─ page.tsx
│     │  │     ├─ (docs)
│     │  │     │  ├─ docs
│     │  │     │  │  ├─ layout.tsx
│     │  │     │  │  └─ [[...slug]]
│     │  │     │  │     └─ page.tsx
│     │  │     │  └─ layout.tsx
│     │  │     ├─ (editor)
│     │  │     │  └─ editor
│     │  │     │     ├─ cluster
│     │  │     │     │  └─ [clusterId]
│     │  │     │     │     └─ page.tsx
│     │  │     │     └─ layout.tsx
│     │  │     └─ (marketing)
│     │  │        ├─ blog
│     │  │        │  ├─ page.tsx
│     │  │        │  └─ [...slug]
│     │  │        │     └─ page.tsx
│     │  │        ├─ layout.tsx
│     │  │        ├─ page.tsx
│     │  │        └─ pricing
│     │  │           ├─ loading.tsx
│     │  │           └─ page.tsx
│     │  ├─ components
│     │  │  ├─ base-item.tsx
│     │  │  ├─ billing-form.tsx
│     │  │  ├─ blog
│     │  │  │  └─ blog-posts.tsx
│     │  │  ├─ blog-card.tsx
│     │  │  ├─ card-hover-effect.tsx
│     │  │  ├─ card-skeleton.tsx
│     │  │  ├─ code-copy.tsx
│     │  │  ├─ comments.tsx
│     │  │  ├─ content
│     │  │  │  ├─ mdx-card.tsx
│     │  │  │  ├─ mdx-components.tsx
│     │  │  │  └─ toc.tsx
│     │  │  ├─ docs
│     │  │  │  ├─ page-header.tsx
│     │  │  │  ├─ pager.tsx
│     │  │  │  ├─ search.tsx
│     │  │  │  └─ sidebar-nav.tsx
│     │  │  ├─ document-guide.tsx
│     │  │  ├─ empty-placeholder.tsx
│     │  │  ├─ features-card.tsx
│     │  │  ├─ features-grid.tsx
│     │  │  ├─ github-star.tsx
│     │  │  ├─ header.tsx
│     │  │  ├─ infiniteMovingCards.tsx
│     │  │  ├─ k8s
│     │  │  │  ├─ cluster-config.tsx
│     │  │  │  ├─ cluster-create-button.tsx
│     │  │  │  ├─ cluster-item.tsx
│     │  │  │  └─ cluster-operation.tsx
│     │  │  ├─ locale-change.tsx
│     │  │  ├─ main-nav.tsx
│     │  │  ├─ meteors-card.tsx
│     │  │  ├─ mobile-nav.tsx
│     │  │  ├─ modal-provider.tsx
│     │  │  ├─ modal.tsx
│     │  │  ├─ mode-toggle.tsx
│     │  │  ├─ nav.tsx
│     │  │  ├─ navbar.tsx
│     │  │  ├─ price
│     │  │  │  ├─ billing-form-button.tsx
│     │  │  │  ├─ pricing-cards.tsx
│     │  │  │  └─ pricing-faq.tsx
│     │  │  ├─ questions.tsx
│     │  │  ├─ rightside-marketing.tsx
│     │  │  ├─ shell.tsx
│     │  │  ├─ shimmer-button.tsx
│     │  │  ├─ sign-in-modal-clerk.tsx
│     │  │  ├─ sign-in-modal.tsx
│     │  │  ├─ site-footer.tsx
│     │  │  ├─ sparkles.tsx
│     │  │  ├─ tailwind-indicator.tsx
│     │  │  ├─ textGenerateEffect.tsx
│     │  │  ├─ theme-provider.tsx
│     │  │  ├─ theme-toggle.tsx
│     │  │  ├─ typewriterEffectSmooth.tsx
│     │  │  ├─ user-account-nav.tsx
│     │  │  ├─ user-auth-form.tsx
│     │  │  ├─ user-avatar.tsx
│     │  │  ├─ user-clerk-auth-form.tsx
│     │  │  ├─ user-name-form.tsx
│     │  │  ├─ video-scroll.tsx
│     │  │  ├─ wobble.tsx
│     │  │  └─ word-reveal.tsx
│     │  ├─ config
│     │  │  ├─ dictionaries
│     │  │  │  ├─ en.json
│     │  │  │  ├─ ja.json
│     │  │  │  ├─ ko.json
│     │  │  │  └─ zh.json
│     │  │  ├─ i18n-config.ts
│     │  │  ├─ ph-config.ts
│     │  │  ├─ price
│     │  │  │  ├─ price-data.ts
│     │  │  │  └─ price-faq-data.ts
│     │  │  ├─ providers.tsx
│     │  │  ├─ site.ts
│     │  │  └─ ui
│     │  │     ├─ dashboard.ts
│     │  │     ├─ docs.ts
│     │  │     └─ marketing.ts
│     │  ├─ content
│     │  │  ├─ authors
│     │  │  │  └─ nok8s.mdx
│     │  │  ├─ blog
│     │  │  │  ├─ deploying-next-apps.mdx
│     │  │  │  ├─ dynamic-routing-static-regeneration.mdx
│     │  │  │  ├─ preview-mode-headless-cms.mdx
│     │  │  │  └─ server-client-components.mdx
│     │  │  ├─ docs
│     │  │  │  ├─ documentation
│     │  │  │  │  └─ index.mdx
│     │  │  │  ├─ in-progress.mdx
│     │  │  │  └─ index.mdx
│     │  │  └─ guides
│     │  │     └─ using-next-auth-next-14.mdx
│     │  ├─ env.mjs
│     │  ├─ hooks
│     │  │  ├─ use-lock-body.ts
│     │  │  ├─ use-media-query.ts
│     │  │  ├─ use-mounted.ts
│     │  │  ├─ use-scroll.ts
│     │  │  └─ use-signin-modal.ts
│     │  ├─ lib
│     │  │  ├─ currency.ts
│     │  │  ├─ generate-pattern.ts
│     │  │  ├─ get-dictionary.ts
│     │  │  ├─ toc.ts
│     │  │  ├─ use-debounce.tsx
│     │  │  ├─ use-mounted.ts
│     │  │  ├─ utils.ts
│     │  │  ├─ validations
│     │  │  │  └─ user.ts
│     │  │  └─ zod-form.tsx
│     │  ├─ middleware.ts
│     │  ├─ styles
│     │  │  ├─ calsans.ttf
│     │  │  ├─ fonts
│     │  │  │  ├─ CalSans-SemiBold.ttf
│     │  │  │  ├─ CalSans-SemiBold.woff
│     │  │  │  ├─ CalSans-SemiBold.woff2
│     │  │  │  ├─ Inter-Bold.ttf
│     │  │  │  └─ Inter-Regular.ttf
│     │  │  ├─ globals.css
│     │  │  ├─ mdx.css
│     │  │  └─ theme
│     │  │     └─ default.css
│     │  ├─ trpc
│     │  │  ├─ client.ts
│     │  │  ├─ server.ts
│     │  │  └─ shared.ts
│     │  ├─ types
│     │  │  ├─ globals.d.ts
│     │  │  ├─ index.d.ts
│     │  │  ├─ k8s.d.ts
│     │  │  ├─ meteors.d.ts
│     │  │  └─ next-auth.d.ts
│     │  └─ utils
│     │     ├─ api.ts
│     │     ├─ clerk.ts
│     │     └─ nextauth.ts
│     ├─ tailwind.config.ts
│     └─ tsconfig.json
├─ bun.lockb
├─ clerk.png
├─ CODE_OF_CONDUCT.md
├─ CONTRIBUTING.md
├─ directory.md
├─ LICENSE
├─ package.json
├─ packages
│  ├─ api
│  │  ├─ .eslintignore
│  │  ├─ package.json
│  │  ├─ src
│  │  │  ├─ edge.ts
│  │  │  ├─ env.mjs
│  │  │  ├─ index.ts
│  │  │  ├─ root.ts
│  │  │  ├─ router
│  │  │  │  ├─ auth.ts
│  │  │  │  ├─ customer.ts
│  │  │  │  ├─ health_check.ts
│  │  │  │  ├─ k8s.ts
│  │  │  │  └─ stripe.ts
│  │  │  ├─ transformer.ts
│  │  │  └─ trpc.ts
│  │  └─ tsconfig.json
│  ├─ auth
│  │  ├─ .eslintignore
│  │  ├─ .prettierignore
│  │  ├─ clerk.ts
│  │  ├─ db.ts
│  │  ├─ env.mjs
│  │  ├─ index.ts
│  │  ├─ nextauth.ts
│  │  ├─ package.json
│  │  └─ tsconfig.json
│  ├─ common
│  │  ├─ .eslintignore
│  │  ├─ package.json
│  │  ├─ src
│  │  │  ├─ config
│  │  │  │  └─ site.ts
│  │  │  ├─ email.ts
│  │  │  ├─ emails
│  │  │  │  └─ magic-link-email.tsx
│  │  │  ├─ env.mjs
│  │  │  ├─ index.ts
│  │  │  └─ subscriptions.ts
│  │  └─ tsconfig.json
│  ├─ db
│  │  ├─ index.ts
│  │  ├─ package.json
│  │  ├─ prisma
│  │  │  ├─ enums.ts
│  │  │  ├─ README.md
│  │  │  ├─ schema.prisma
│  │  │  └─ types.ts
│  │  └─ tsconfig.json
│  ├─ stripe
│  │  ├─ .eslintignore
│  │  ├─ package.json
│  │  ├─ src
│  │  │  ├─ env.mjs
│  │  │  ├─ index.ts
│  │  │  ├─ plans.ts
│  │  │  └─ webhooks.ts
│  │  └─ tsconfig.json
│  └─ ui
│     ├─ .eslintignore
│     ├─ package.json
│     ├─ src
│     │  ├─ 3d-card.tsx
│     │  ├─ accordion.tsx
│     │  ├─ alert-dialog.tsx
│     │  ├─ alert.tsx
│     │  ├─ animated-gradient-text.tsx
│     │  ├─ animated-list.tsx
│     │  ├─ animated-tooltip.tsx
│     │  ├─ avatar.tsx
│     │  ├─ background-lines.tsx
│     │  ├─ button.tsx
│     │  ├─ calendar.tsx
│     │  ├─ callout.tsx
│     │  ├─ card-hover-effect.tsx
│     │  ├─ card-skeleton.tsx
│     │  ├─ card.tsx
│     │  ├─ checkbox.tsx
│     │  ├─ colorful-text.tsx
│     │  ├─ command.tsx
│     │  ├─ container-scroll-animation.tsx
│     │  ├─ data
│     │  │  └─ globe.json
│     │  ├─ data-table.tsx
│     │  ├─ dialog.tsx
│     │  ├─ dropdown-menu.tsx
│     │  ├─ following-pointer.tsx
│     │  ├─ form.tsx
│     │  ├─ glowing-effect.tsx
│     │  ├─ icons.tsx
│     │  ├─ index.ts
│     │  ├─ infinite-moving-cards.tsx
│     │  ├─ input.tsx
│     │  ├─ label.tsx
│     │  ├─ marquee.tsx
│     │  ├─ meteors.tsx
│     │  ├─ popover.tsx
│     │  ├─ scroll-area.tsx
│     │  ├─ select.tsx
│     │  ├─ sheet.tsx
│     │  ├─ skeleton.tsx
│     │  ├─ sparkles.tsx
│     │  ├─ switch.tsx
│     │  ├─ table.tsx
│     │  ├─ tabs.tsx
│     │  ├─ text-generate-effect.tsx
│     │  ├─ text-reveal.tsx
│     │  ├─ toast.tsx
│     │  ├─ toaster.tsx
│     │  ├─ typewriter-effect.tsx
│     │  ├─ use-toast.tsx
│     │  ├─ utils
│     │  │  └─ cn.ts
│     │  └─ wobble-card.tsx
│     ├─ tailwind.config.ts
│     └─ tsconfig.json
├─ README.md
├─ README_de.md
├─ README_vi.md
├─ README_zh.md
├─ saasfly-logo.svg
├─ SECURITY.md
├─ setupyourpay.png
├─ tailwind.config.js
├─ tooling
│  ├─ eslint-config
│  │  ├─ base.js
│  │  ├─ nextjs.js
│  │  ├─ package.json
│  │  ├─ react.js
│  │  └─ tsconfig.json
│  ├─ prettier-config
│  │  ├─ index.mjs
│  │  ├─ package.json
│  │  └─ tsconfig.json
│  ├─ tailwind-config
│  │  ├─ .eslintignore
│  │  ├─ index.ts
│  │  ├─ package.json
│  │  ├─ postcss.js
│  │  └─ tsconfig.json
│  └─ typescript-config
│     ├─ base.json
│     └─ package.json
├─ turbo
│  └─ generators
│     ├─ config.ts
│     └─ templates
│        ├─ package.json.hbs
│        └─ tsconfig.json.hbs
├─ turbo.json
├─ twillot.png
└─ vercel.json

```
