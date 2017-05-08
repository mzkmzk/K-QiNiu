# K-Qiniu

将webpack打包后的文件上传至七牛云


# Install

npm:

```
  npm install k-qiniu --save
```


# Use

```
  var QiniuPlugin = reqiure('k-qiniu'),
     qiniuPlugin = new QiniuPlugin({

    // 七牛云的两对密匙 Access Key & Secret Key
    accessKey: 'accessKey',
	
    secretKey: 'secretKey',
	
    // 七牛云存储空间名称
    bucket: 'test',
    
    // 上传到七牛后保存的文件名
    path: 'rc/[name]/[version]/[asset]'

  });

  // Webpack 配置文件
  module.exports = {
    plugins: [
      qiniuPlugin
      // ...
    ]
    // ...
  };

```

