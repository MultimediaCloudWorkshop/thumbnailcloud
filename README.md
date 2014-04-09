# 图像缩略图云  

发送图像URL，返回缩略图    

（试运营）  
  
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
  - Auto Scaling & Load Balance (试运营期间暂不提供) 
  - AWS Cloud Native
  - GraphicsMagick Core
  - 图像和缩略图双层缓存
  - Open Source
- 价廉  
  - 仅根据请求次数收费，无其他收费
  - 每次请求1分钱
  - 当前免费试用

### 使用
- URL
  - http://multimediaapi.elasticbeanstalk.com/image/thumbnail
  - GET 方法
- 参数
  - url: 图像URL   
  - width: 缩略图宽度 （可选）  
  - height: 缩略图高度 （可选）  
  - crop: 裁剪方式 （可选）  
    - Center: 居中裁剪
    - North: 从顶部裁剪
  - apikey: API key (请发送邮件到 multimediacloudworkshop@gmail.com，免费申请)
- 返回
  - 成功，返回缩略图文件
  - 失败，返回JSON格式错误信息
- 注意  
  - 图像URL需进行URL编码  
  - 参数width和height不能同时缺省  
  - 参数apikey必须为有效的API Key   
  - 缩略图格式(Content-Type)与图像格式一致  

### 示例  
- 图像URL：http://upload.wikimedia.org/wikipedia/commons/6/6b/SelbstPortrait_VG2.jpg  
- 已编码的图像URL：http%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F6%2F6b%2FSelbstPortrait_VG2.jpg  
- 缩略图：宽100像素，高100像素，居中裁剪 
- 请求URL：http://multimediaapi.elasticbeanstalk.com/image/thumbnail?url=http%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F6%2F6b%2FSelbstPortrait_VG2.jpg&width=100&height=100&crop=Center&apikey=YourAPIKey
- 用你的API Key替换掉上面请求中的 YourAPIKey

### 价格  
- 当前试运营：免费  
- 正式运营：0.01元RMB/请求  

### 联系  
- 邮件：multimediacloudworkshop@gmail.com  
- 如果您需要缩略图私有云，欢迎联系我们
- 如果您有其他需求，欢迎联系我们  

