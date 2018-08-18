# 阿里云oss部署

# 启动方式

- 在home目录下新建`/kong/frontend/secret/index.js`文件，模板如下：
```
module.exports = {
  aliOSS: {
    accessKeyId: "ACCESSKEYID",
    accessKeySecret: "ACCESSKEYSECRET",
    roleArn: 'ROLEARN'
  }
}
```

- 运行命令

`node index.js [本地文件所在目录] [bucket名称]`

上传成功后，会保持`[本地文件所在目录]`的目录结构