# git 开启代理和取消代理

## git 开启代理和取消代理

同时使用 GitHub 和 Gitee，要设置 git 代理配置，在使用 GitHub 时开启代理，使用 Gitee 时取消代理，才能正常进行 git 操作

* git 开启代理

```bash
git config --global http.proxy http://127.0.0.1:7890
git config --global https.proxy http://127.0.0.1:7890
```

* git 取消代理

```bash
git config --global --unset http.proxy
git config --global --unset https.proxy
```