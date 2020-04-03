# CDN
静态资源
## jsDeliver+npm
jsDeliver+npm就是把npm上的包当做cdn的存储。
使用教程：（jsDeliver不支持加载超过20M的资源，所以一些视频最好压缩到20M以下）
```javascript
// load any project hosted on npm
// 加载以NPM为存储的任何项目
https://cdn.jsdelivr.net/npm/package@version/file
// load jQuery v3.2.1
// 比如加载Jquery3.2.1
https://cdn.jsdelivr.net/npm/jquery@3.2.1/dist/jquery.min.js
// use a version range instead of a specific version
//使用版本范围而不是特定版本
https://cdn.jsdelivr.net/npm/jquery@3.2/dist/jquery.min.js
https://cdn.jsdelivr.net/npm/jquery@3/dist/jquery.min.js
// omit the version completely to get the latest one
//完全忽略版本以获取最新版本，不建议使用
https://cdn.jsdelivr.net/npm/jquery/dist/jquery.min.js
```

## jsDeliver+github
```javascript
https://cdn.jsdelivr.net/gh/你的用户名/你的仓库名@发布的版本号/文件路径
//加载图片
https://cdn.jsdelivr.net/gh/Zevs6/CDN/img/avatar.jpg

//注意：版本号不是必需的，是为了区分新旧资源，如果不使用版本号，将会直接引用最新资源，除此之外还可以使用某个范围内的版本，查看所有资源等，具体使用方法如下：

    // 加载任何Github发布、提交或分支
    https://cdn.jsdelivr.net/gh/user/repo@version/file
    // 加载 jQuery v3.2.1
    https://cdn.jsdelivr.net/gh/jquery/jquery@3.2.1/dist/jquery.min.js
    // 使用版本范围而不是特定版本
    https://cdn.jsdelivr.net/gh/jquery/jquery@3.2/dist/jquery.min.js
    https://cdn.jsdelivr.net/gh/jquery/jquery@3/dist/jquery.min.js
    // 完全省略该版本以获取最新版本
    https://cdn.jsdelivr.net/gh/jquery/jquery/dist/jquery.min.js
    // 将“.min”添加到任何JS/CSS文件中以获取缩小版本，如果不存在，将为会自动生成
    https://cdn.jsdelivr.net/gh/jquery/jquery@3.2.1/src/core.min.js
    // 在末尾添加 / 以获取资源目录列表
    https://cdn.jsdelivr.net/gh/jquery/jquery/

```

## jsDeliver+WordPress
WordPress是一款个人博客系统，并逐步演化成一款内容管理系统软件，它是使用PHP语言和MySQL数据库开发的。用户可以在支持 PHP 和 MySQL数据库的服务器上使用自己的博客。
jsDeliver+WordPress使用教程：
```javascript
// load any plugin from the WordPress.org plugins SVN repo
// 从WordPress.org等SVN仓库加载任何插件
https://cdn.jsdelivr.net/wp/plugins/project/tags/version/file
```
