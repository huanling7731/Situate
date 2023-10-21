# 项目地址

https://github.com/huanling7731/Situate
git commit -m ""
git push origin main

# 相关命令
rz 上传
sz 下载
unzip
systemctl restart httpd.service 这个是重启的命令
systemctl status httpd.service 这个能查到是否启动成功
其他方式上传 https://cloud.tencent.com/document/product/213/2133

# 替换数据详细步骤

1. 打开机器地址（https://console.cloud.tencent.com/cvm/instance/index?rid=4），点击右侧登录
![示例](http://www.situatearchitecture.com/static/img/steps/1.png)
2. 在弹出框输入密码：R5U2uLAcxhTN
![示例](http://www.situatearchitecture.com/static/img/steps//2.png)
3. 在命令行输入以下命令，更新数据文件，执行完一次rz刷新页面可看到新效果
```
    cd /var/www/html/data // 切换到数据目录
    rz -y // 上传新的projectList.json更新项目页数据，上传新的mediaList.json更新媒体页数据数据
```
![示例](http://www.situatearchitecture.com/static/img/steps//4.png)
4. 在命令行输入以下命令，更新图片，执行完一次rz刷新页面可看到新效果
```
    cd /var/www/html/static/img/project // 如果需要更换项目页图片，切换到项目页图片目录
    rz -y // 上传新文件，对应json中的图片名
    cd /var/www/html/static/img/media // 如果需要更换媒体页图片，切换到媒体页图片目录
    rz -y // 上传新文件，对应json中的图片名
```
![示例](http://www.situatearchitecture.com/static/img/steps//5.png)

# 数据格式

```
{
    "id": 1,
    "projectName": "项目名称",
    "projectNameEn": "项目英文名称",
    "projectDes": "项目描述，原网页中是年份，如果不需要可以不写，也可以替换成其他简短的描述",
    "projectImg": "图片名称.后缀，最好是英文无特殊字符，不需要太大，这个页面图片较多，太大影响性能，pad屏幕可清晰展示即可，如果没有小的可以统一给我大的，最后批量压缩",
    "projectUrl": "公众号链接"
}
```

命名规范：字体和图片命名为首字母大写加下划线，如Cera_Pro_Light
每种字体不同给一份统一的文件，不用区分粗细斜体，文件格式包括woff2、woff、ttf、svg、eot

# 相关地址

https://www.vectorarchitects.com/projects
http://www.situatearchitecture.com/list.html
https://www.swiper.com.cn/api/index.html