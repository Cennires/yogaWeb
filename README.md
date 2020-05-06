一、数据库设计

|   表名   |                            属性                             |
| :------: | :---------------------------------------------------------: |
| Profile  |                 user ：一对一属性，对应User                 |
|          |           image ：models.ImageField，用户头像路径           |
|   Post   |            title：models.CharField，上传照片名称            |
|          |           image： models.ImageField，上传照片路径           |
|          |       date_published ：models.DateTimeField，上传时间       |
|          |                 author ：外键属性，对应User                 |
|   Yoga   |           img ： models.ImageField，瑜伽图片路径            |
|          | level ： models.IntegerField，瑜伽难度（1，2，3，依次递增） |
|          |            title：models.CharField，上传照片名称            |
| DownYoga |       image：models.ImageField，瑜伽返回结果图片路径        |
|          |       jsonFile ： models.FileField，瑜伽返回json文件        |
|          |  upPost ： models.ForeignKey，外键属性，与瑜伽标准图片对应  |

二、主要功能

首页瑜伽展示（初级、中级、高级）----->注册----->登录

用户：更改用户名、邮箱、头像，历史记录，上传照片，查看评测结果

