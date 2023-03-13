# github 配置pagehost
    deploy 域名恢复过来了 CNAME 放到 更目录的 source下面
    https://micro.blog.csdn.net/article/details/80177787
    https://blog.csdn.net/weixin_41747528/article/details/102772937
    https://blog.csdn.net/i_do_not_know_you/article/details/105594269
    The hostname of the origin is unresolvable (DNS) or blocked by policy
    正确的解决方案
    首先奉上官方指路文档，按照绑定顶尖域名的方式来解析你的域名Configuring an apex domain。
    不要企图通过ping的方式，来找出所有的IP地址。因为你的网站的IP是会变化的哦。所以你需要添加这四个解析到IP地址的A记录。
    185.199.108.153
    185.199.109.153
    185.199.110.153
    185.199.111.153

# 软件
    https://netlify.app/     
    https://www.tidio.com/
    https://livere.com/

# hexo配置
    https://github.com/wnwd/hexo-asset-pro 解决 图片在markdown中可以显示，但是在server中不显示的问题 ，
    hexo-renderer-marked/lib/renderer.js
    // 替换 第一层路径
    // artookitx-build/img.png
    // img.png
    if (!/^(#|\/\/|http(s)?:)/.test(href) && !relative_link ) {
    // href = href.substring(href.indexOf("/")+1)
    }
    Typora 中图片设置 ，图片选项中，插入图片时选择 【选择复制到指定目录】 ./${filename}/ 

# 源码站点
    https://github.com/hnlzwaq/homespace.git
    https://gitee.com/hnlzwaq/homespace.git
    https://e.coding.net/hnlzwaq/my/homespace.git
# 发布站点
    https://gitee.com/hnlzwaq/hnlzwaq.git
    ttps://github.com/hnlzwaq/hnlzwaq.github.io.git

# 所有站点
[mingyue.today](https://mingyue.today/)

[hnlzwaq.gitee.io](https://hnlzwaq.gitee.io/)

[hnlzwaq.github.io](https://hnlzwaq.github.io/)

[netlify](https://effortless-panda-50bb23.netlify.app/)

# 操作
```shell
 hexo new opencv-stitch-hd-areas
 hexo publish opencv-stitch-hd-areas
```

# 启动
```shell
    hexo clean ; hexo server
```
