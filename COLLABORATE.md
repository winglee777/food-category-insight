# 协作部署指南

欢迎加入！这份文档帮你快速上手。

---

## 一次性准备（5 分钟）

### 1. 接受邀请

在邮箱里找 GitHub 邀请邮件，点 **Accept invitation** 接受 collaborator 权限。

### 2. 装好 git

- **Mac**：自带，跳过此步
- **Windows**：https://git-scm.com/download/win

### 3. 克隆仓库

打开终端 / 命令行：

```bash
git clone https://github.com/winglee777/food-category-insight.git
cd food-category-insight

# 配置一下身份（首次）
git config user.name "你的名字"
git config user.email "你的GitHub邮箱"
```

---

## 日常改一次部署一次（每次 30 秒）

```bash
# 1. 进入仓库目录
cd food-category-insight

# 2. 拉一下最新代码（避免冲突）
git pull

# 3. 用任意编辑器改 index.html 或其他文件
#    （VSCode / Sublime / 记事本都行）

# 4. 改完保存后，三连命令推送
git add .
git commit -m "简单写一句改了什么"
git push
```

首次 `git push` 时会让你登录 GitHub，用你自己的账号登录即可（Mac 会自动存到 keychain，下次不用再登）。

---

## 部署效果查看

push 成功后等 **30-60 秒**，访问下面网址（强制刷新 Cmd+Shift+R）：

👉 https://winglee777.github.io/food-category-insight/

---

## 文件结构说明

```
food-category-insight/
├── index.html                  # 主页：总经理汇报 OnePage
├── case-shamo-tigernut.html    # 沙漠一号·虎坚果案例页
├── assets/                     # 长图素材
│   ├── duanwu-longimage.png    # 端午长图
│   ├── q3-longimage.png        # Q3 长图
│   ├── q4-longimage.png        # Q4 长图
│   └── case-shamo-longimage.png # 沙漠一号案例长图
└── COLLABORATE.md              # 本文档
```

---

## 常见问题

**Q: push 时报错 `Permission denied`？**
A: 邀请没接受，去邮箱点 Accept invitation。

**Q: push 时报错 `Updates were rejected`？**
A: 别人先 push 了，先 `git pull` 拉最新，再 `git push`。

**Q: 改完 push 了但网址没更新？**
A: 等 1-2 分钟，GitHub Pages 后台需要时间重建；强制刷新浏览器（Cmd+Shift+R / Ctrl+F5）。

**Q: 想看部署状态？**
A: 进 https://github.com/winglee777/food-category-insight/actions 看最新一次构建是绿色对号（成功）还是红色叉（失败）。

---

## 卡住的话

直接把报错截图发我。
