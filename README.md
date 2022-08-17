# Nuxt 3 Minimal Starter

Look at the [nuxt 3 documentation](https://v3.nuxtjs.org) to learn more.

## Setup

Make sure to install the dependencies:

```bash
# yarn
yarn install

# npm
npm install

# pnpm
pnpm install --shamefully-hoist
```

## Development Server

Start the development server on http://localhost:3000

```bash
npm run dev
```

## Production

Build the application for production:

```bash
npm run build
```

Locally preview production build:

```bash
npm run preview
```

Checkout the [deployment documentation](https://v3.nuxtjs.org/guide/deploy/presets) for more information.

## 目录

- .nuxt // 自动生成的目录，用于展示结果
- node_modules // 项目依赖包存放目录
- .gitignore // Git的配置目录，比如一些文件不用Git管理就可以在这个文件中配置
- app.vue // 项目入口文件，你可以在这里配置路由的出口
- nuxt.config.ts // nuxt项目的配置文件 ，这个里边可以配置Nuxt项目的方法面面
- package-lock.json // 锁定安装时包的版本，以保证其他人在 npm install时和你保持一致
- package.json // 包的配置文件和项目的启动调式命令配置
- README.md // 项目的说明文件
- tsconfig.json // TypeScript的配置文件
- pages // 开发的页面目录
- components // 组件目录
- assets // 静态资源目录
- layouts // 项目布局目录
- composables //模块化全局代码
- middleware //路由中间件
