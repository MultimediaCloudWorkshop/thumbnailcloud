# 图像缩略图云  Image Thumbnail Cloud

发送图像URL 返回缩略图

### 特点

- 简单
  - 发送GET请求
  - 返回缩略图文件
- 实时
  - 即请求即获得
- 多种缩略图模式  
  - 限定宽度，等比例缩放
  - 限定高度，等比例缩放
  - 限定宽度和高度，等比例缩放
  - 限定宽度和高度，居中裁剪
  - 限定宽度和高度，从顶部裁剪
- 稳定
  - Auto Scaling & Load Balance  
  - AWS Cloud Native
  - GraphicsMagick Core
  - 图像和缩略图双层缓存
  - Open Source
- 专注
  - 只创建缩略图
  - 不存储图像和缩略图

### 使用

- URL
  - http://multimediacloud.elasticbeanstalk.com/image/thumbnail
  - GET 方法
- 参数
  - url: 图像URL   
  - width: 缩略图宽度 （可选）  
  - height: 缩略图高度 （可选）  
  - crop: 裁剪方式 （可选）  
    - Center: 居中裁剪
    - North: 从顶部裁剪
  - apikey: API key (请发送邮件到 thumbnailcloud@gmail.com，免费申请)
- 返回
  - 成功，返回缩略图文件
  - 失败，返回JSON格式错误信息
- 注意  
  - 图像URL需进行URL编码  
  - 参数width和height不能同时缺失  
  - 参数apikey必须为有效的API Key   
  - 缩略图格式(Content-Type)与图像格式一致  

### 价格  

- 当前**免费试用**  
- 将来按照请求次数收费  
