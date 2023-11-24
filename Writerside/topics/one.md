# Blog

## Freenom 解析控制台

### 1. 要创建 A 记录，请将您的顶点域指向 GitHub Pages 的 IP 地址。

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

### 2. 要创建 AAAA 记录，请将您的顶点域指向 GitHub Pages 的 IP 地址。

```
2606:50c0:8000::153
2606:50c0:8001::153
2606:50c0:8002::153
2606:50c0:8003::153
```

### 3. 对于 www 子域，我创建了一个 CNAME 记录，将"host"设置为"www" ,将”data“设置为 zlx.github.io 。

![freenom](freenom.png){ width=700 }{border-effect=line}

### 4. 在 GitHub Pages 配置如下 :

![github](github.png){ width=700 }{border-effect=line}

### 5. 打包发布, 解析放到docs目录下

CNAME 文件不能删除

<seealso>
    <category ref="wrs">
        <a href="https://medium.com/@isphinxs/using-a-custom-domain-name-with-github-pages-c9cdc2084d54">Using a Custom Domain Name with GitHub Pages</a>
    </category>
</seealso>
