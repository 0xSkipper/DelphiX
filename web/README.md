# DelphiX-web

## next-cli

### 环境要求

node -v # => v20.0.0+
npm -v # => 10.0.0+
npx -v # => 10.0.0+

### 安装

npx create-next-app@14.0.4

| Option        | Value |
|---------------|-------|
| project named | web   |
| TypeScript    | Yes   |
| ESLint        | Yes   |
| Tailwind      | Yes   |
| src/directory | No    |
| App Router    | No    |
| alias         | No    |

cd web
npm i
npm i antd @ant-design/web3 --save
npm install antd --save
npm i @ant-design/web3-wagmi wagmi viem @tanstack/react-query --save
npm i viem --save

### 配置

next.config.js中添加

```js
/** @type {import('next').NextConfig} */
const nextConfig = {
    reactStrictMode: true,
// + swcMinify: true,
// + transpilePackages: ["@ant-design", "antd", "rc-util", "rc-pagination", "rc-picker"],
  }

export default nextConfig
```

globals.css中添加

```css
body {
  /* + min-height: 100vh;*/
  color: rgb(var(--foreground-rgb));
  background: linear-gradient(
      to bottom,
      transparent,
      rgb(var(--background-end-rgb))
  ) rgb(var(--background-start-rgb));
}
```

### 运行

npm run dev 或 IDE的package.json的dev脚本Button

