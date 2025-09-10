# trae 前端高效开发设置指南

## 1. 环境准备

- 推荐使用 [VS Code](https://code.visualstudio.com/) 作为主要开发工具。
- 安装 Node.js（建议版本：18.x 及以上），可通过 [nvm](https://github.com/nvm-sh/nvm) 管理多版本。
- 推荐使用 pnpm 作为包管理工具：
  ```bash
  npm install -g pnpm
  ```
- 克隆项目代码：
  ```bash
  git clone <项目仓库地址>
  cd <项目目录>
  ```
- 安装依赖：
  ```bash
  pnpm install
  ```

## 2. 推荐 VS Code 插件

- ESLint
- Prettier
- Volar（Vue3 支持）
- GitLens
- vscode-icons

## 3. 常用开发命令

- 启动开发环境：
  ```bash
  pnpm dev
  ```
- 构建生产包：
  ```bash
  pnpm build
  ```
- 代码格式化：
  ```bash
  pnpm format
  ```
- 运行单元测试：
  ```bash
  pnpm test
  ```

## 4. 代码规范与提交

- 遵循项目内的 ESLint 和 Prettier 配置，保存时自动格式化。
- 使用 Git 进行分支管理，建议采用 feature/xxx 命名规范。
- 提交信息建议遵循 [Conventional Commits](https://www.conventionalcommits.org/zh-hans/v1.0.0/) 规范。

## 5. 性能与效率提升建议

- 善用 VS Code 快捷键和多光标编辑。
- 利用 Volar 实现更好的 Vue3 类型提示和跳转。
- 推荐使用 pnpm 的 workspace 功能进行多包管理。
- 合理拆分组件，提升复用性和可维护性。

## 6. 常见问题排查

- 依赖安装异常：尝试删除 `node_modules` 和 `pnpm-lock.yaml` 后重新安装。
- 端口被占用：修改 `vite.config.ts` 中的端口配置或释放端口。
- 类型报错：确认 TypeScript 版本与依赖兼容。

---

如有更多问题，请查阅项目 README 或联系团队成员。
