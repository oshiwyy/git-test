# git-test

`oshiwyy` 的 Git 全流程连通性测试仓库。

## 这个仓库验证了什么

| 项目 | 值 |
|---|---|
| 鉴权方式 | SSH key（走 `ssh.github.com:443`） |
| 提交身份 | oshiwyy |
| 创建方式 | 本地 `git init` → `commit` → `push` |
| 主机密钥校验 | 使用 GitHub 官方公布的 9 条指纹 |

## 完整流程

```bash
git init -b main
git add .
git commit -m "first commit"
git remote add origin git@github.com:oshiwyy/git-test.git
git push -u origin main
```

## 提交身份验证

第二次提交，改用 GitHub 账号中已验证的主邮箱，用于验证 commit 归属。
