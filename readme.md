
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
————————————————
版权声明：本文为CSDN博主「arbitrary_me」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/i_do_not_know_you/article/details/105594269


hexo g -d

netlify

cloudflare

hexo clean ; hexo g ;hexo d


https://mingyue.today/
https://hnlzwaq.gitee.io/
https://hnlzwaq.github.io/
https://effortless-panda-50bb23.netlify.app/



