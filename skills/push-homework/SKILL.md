---
name: push-homework
description: 一键推送作业到 git 远程仓库 (origin/main)
---

# /push-homework — 推送作业到 Git

自动暂存所有更改，生成提交信息并推送到远程仓库。

---

## 执行流程

### 1. 检查 Git 状态
先用 `git status` 检查是否有更改需要推送。

### 2. 暂存所有更改
```
git add -A
```

### 3. 生成提交信息
自动生成格式：`push homework YYYY-MM-DD HH:MM`

### 4. 提交
```
git commit -m "push homework YYYY-MM-DD HH:MM"
```

### 5. 推送到远程
```
git push origin main
```

---

## 注意事项

- 使用 `git push -u origin main` 首次推送并设置上游分支
- 如果当前分支不是 main，会推送当前分支到同名的远程分支
- 建议推送前确认没有敏感文件被意外提交

---

## 使用方式

直接输入：
```
/push-homework
```
