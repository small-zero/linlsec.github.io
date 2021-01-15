# GitHub无法加载图片

**GitHub无法加载图片，是因为DNS被污染，因此，需要我们手动配置一下方可显示**

**配置前：没有加载出图片**

![1](https://github.com/linl-sec/linlsec.github.io/tree/main/images/%E6%97%A5%E5%B8%B8%E6%93%8D%E4%BD%9C%E9%85%8D%E7%BD%AE/1.png)

**配置后：图片加载成功**

![2](https://github.com/linl-sec/linlsec.github.io/tree/main/images/%E6%97%A5%E5%B8%B8%E6%93%8D%E4%BD%9C%E9%85%8D%E7%BD%AE/2.png)

**如何配置：**

**将以下内容复制粘贴到hosts文件中：**

```shell
# GitHub Start
140.82.114.3    github.com
140.82.112.3    gist.github.com
140.82.112.6    api.github.com
185.199.108.153    assets-cdn.github.com
199.232.68.133    raw.githubusercontent.com
199.232.68.133    gist.githubusercontent.com
199.232.68.133    cloud.githubusercontent.com
199.232.68.133    camo.githubusercontent.com
199.232.68.133    avatars0.githubusercontent.com
199.232.68.133    avatars1.githubusercontent.com
199.232.68.133    avatars2.githubusercontent.com
199.232.68.133    avatars3.githubusercontent.com
199.232.68.133    avatars4.githubusercontent.com
199.232.68.133    avatars5.githubusercontent.com
199.232.68.133    avatars6.githubusercontent.com
199.232.68.133    avatars7.githubusercontent.com
199.232.68.133    avatars8.githubusercontent.com
 # GitHub End
```

```shell
# Windows系统hosts文件位置： C:/Windows/system32/drivers/etc/hosts
# Linux/macOS系统hosts文件位置: /etc/hosts
```

**大功告成！**

