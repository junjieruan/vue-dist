# vue-dist
将本地的vue项目发布到线上

## 修改打包路径
```bash
# 将config文件夹下的index.js文件中build的assetsPublicPath属性改为./(注意不要改成dev的路径)
assetsPublicPath: './'
```
## 打包
```bash
# 在项目路径下执行以下指令，会生成一个dist文件夹，里面包含static文件夹和index.html
npm run build
```

## 上传
```bash
# 在github中新建一个仓库,将打包生成的dist文件夹中的内容上传到github的一个仓库中,此时仓库目录应如下,index.html在根目录 
  -statis
  -.gitattributes
  -index.html
```

## 设置github pages
```bash
# 将对应仓库的setting的github pages选项的source设为master-branch
```


## 预览
```bash
# 再回到setting内的github pages选项处,项目的预览链接已经出现辣!
# 像本vue-dist项目链接就是访问如下链接：
https://junjieruan.github.io/vue-dist/#/
```

## 数据库
```bash
# 此时调用数据库还是失败，要换成访问线上的数据库才行
可通过点击首页的“直接跳转到首页”按钮测试页面的跳转
```
