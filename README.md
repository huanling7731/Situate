# 项目地址

https://github.com/huanling7731/Situate
git commit -m ""
git push origin main

# 部署

机器地址：https://console.cloud.tencent.com/cvm/instance/index?rid=4
pasd：R5U2uLAcxhTN
目录：/var/www/html
相关命令
rz
unzip
systemctl restart httpd.service  这个是重启的命令
systemctl status httpd.service 这个能查到是否启动成功
其他方式上传 https://cloud.tencent.com/document/product/213/2133

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

# 相关地址

https://www.vectorarchitects.com/projects
http://www.situatearchitecture.com/list.html