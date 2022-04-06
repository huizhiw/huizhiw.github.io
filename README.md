# Personal Website built with Hugo


## 经验和总结
This is a simple test for hugo toolchain, I follow this [tutorial](https://cloud.tencent.com/developer/article/1769218) when build the page.

There are some important notes:
1. git clone url & git submodule add url [destination folder]：这两个在使用git add .的时候会有区别
2. config.toml很重要，需要看看使用的themes是否包含了example，方便使用
3. 在config.toml放好以后再创建内容(e.g. hugo new posts/demo.md)才会在content下出现可以显示的内容
4. 用hugo server -D本地预览，预览地址：http://localhost:1313/ 
5. **github pages在静态页面时只支持根目录或者/docs目录，需要使用hugo -d docs将文件导到/docs下在push，同时需要设置GitHub里的settings**
6. 本地仓库->远程仓库，目前顺序
   - 在本地master branch上做修改
   - 修改完checkout -b Verxxx（e.g. checkout -b Ver1.0）存档，留下readme
   - checkout到main线，然后merge master
   - push到远程repo

## to be achieved
1. 如何放入多个themes，在不同themes切换，对content内容的显示会不会有影响
