# 用 Git 保存与同步学习进度

远程仓库：[code_learning_docs](https://github.com/gugugagala/code_learning_docs)。主分支：`main`，使用 SSH 认证。

在仓库根目录运行：

```bash
git status
git diff
# 检查全部修改后暂存；也可以指定需要提交的文件
git add .
git diff --cached
git commit -m "完成 C 001 练习并记录问题"
git push
```

提交说明应描述实际变更，上面的说明只是示例。

查看历史：

```bash
git log --oneline
git show <提交编号>
```

在另一台电脑继续学习：

```bash
git clone git@github.com:gugugagala/code_learning_docs.git
cd code_learning_docs
```

需要先配置该电脑访问 GitHub 的 SSH 认证。已有克隆目录且工作区干净时，开始学习前运行 `git pull --ff-only`。

本地提交后仍需推送才能同步到 GitHub。提交前检查是否包含密码、令牌或私钥；这些内容不要放入仓库。
