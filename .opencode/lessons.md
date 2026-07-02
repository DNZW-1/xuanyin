# 项目教训记录

## GitHub 上传流程

**场景：** 将本地 Gal 项目推到 GitHub

**步骤：**
1. 检查 token 有效性：`Invoke-RestMethod -Uri "https://api.github.com/user" -Headers @{Authorization="token <PAT>"} -Method Get`
2. 创建远程仓库（API）：
   ```
   $body = @{name="xuanyin"; description="..."; private=$false} | ConvertTo-Json
   Invoke-RestMethod -Uri "https://api.github.com/user/repos" -Headers $headers -Body $body -Method Post
   ```
3. 添加 remote 并推送（URL 中内嵌 token 省去交互认证）：
   ```
   git remote add origin https://<USER>:<TOKEN>@github.com/<USER>/<REPO>.git
   git push -u origin master
   ```
4. 推送成功后立即移除 token：
   ```
   git remote set-url origin https://github.com/<USER>/<REPO>.git
   ```

**注意：** token 用完即清，不留存在 remote URL 或文件中。

## Obsidian 文件命名规则（已验证）
见 `.opencode/instructions` 中"文件命名规则"章节。
