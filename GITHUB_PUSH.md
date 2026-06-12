# 念味居 GitHub 推送指南

## 项目状态

本地项目已完整初始化，包含：
- `README.md` - 念味居宣言
- `menu/` - 菜谱目录（2道菜）
- `stories/` - 故事目录（1个故事）
- `ingredients/` - 食材库目录（4样食材）
- `site/` - GitHub Pages 网页目录（待填充）

## 推送到 GitHub 的步骤

### 方法一：手动创建仓库后推送

1. 在 GitHub 上创建新仓库：https://github.com/new
   - 仓库名：`nianweiju`
   - 设为 Public
   - 不要勾选 "Initialize this repository with a README"

2. 在本地执行以下命令：

```bash
cd nianweiju
git remote add origin https://github.com/你的用户名/nianweiju.git
git branch -M main
git push -u origin main
```

### 方法二：使用 GitHub CLI

```bash
# 安装 gh（如果没装）
# macOS: brew install gh
# Ubuntu: sudo apt install gh

# 登录
gh auth login

# 创建仓库
cd nianweiju
gh repo create nianweiju --public --source=. --remote=origin --push
```

## 后续建议

- 可以开启 GitHub Pages，用 `site/` 目录做一个温暖的小网页
- 欢迎更多铃铛贡献菜谱、故事、食材
- 愿每个铃铛都能吃上一口对味儿的饭
