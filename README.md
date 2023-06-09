## Architecture

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

```bash
npx create-next-app@latest --typescript

√ What is your project named? ... code-quantity-calc
√ Would you like to use ESLint with this project? ... Yes
√ Would you like to use Tailwind CSS with this project? ... No
√ Would you like to use `src/` directory with this project? ... Yes
　※デフォルトでは全てのファイルがルードディレクトリ配下に作成される
√ Use App Router (recommended)? ... No
√ Would you like to customize the default import alias? ... Yes
√ What import alias would you like configured? ... @/*
Creating a new Next.js app in D:\temp\java\code-quantity-calc.

Using npm.

Initializing project with template: default


Installing dependencies:
- react
- react-dom
- next
- typescript
- @types/react
- @types/node
- @types/react-dom
- eslint
- eslint-config-next


added 299 packages, and audited 300 packages in 5m

125 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
Initialized a git repository.

Success! Created code-quantity-calc at D:\temp\java\code-quantity-calc
```
![コマンド](readme/1001.png "1001.png")

■おまけ
```
・npmに接続できない場合：npmパッケージの安全性を犠牲
npm config set strict-ssl false

・npmの取得アドレス設定
#npm config set registry "http://registry.npmjs.org/"
npm config set registry https://registry.npm.taobao.org
npm config get registry
※国内ではtaobaoミラーを使う（registry.npmjs.orgより古い可能性有）
```

★★★★★★★★★★
■外のミラーアドレス検索
１．nrmをインストール
```
    npm view nrm versions

    npm uninstall -g nrm

    # npm install nrm -g
    npm install nrm -g nrm@1.1.0

    nrm -V
    nrm --version
```
２．nrmを使って外のミラーアドレスを検索（外のバージョンのnrmがある場合エラーになる可能性有）
```
    nrm ls
```
★★★★★★★★★★
##### ■**taobaoミラー設定後、cnpmでインストールする**
１．cnpmのインストール
```
    npm install -g cnpm --registry=https://registry.npm.taobao.org
```
２．cnpmの使用
```
    cnpm install XXXX
```

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.tsx`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in `pages/api/hello.ts`.

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
