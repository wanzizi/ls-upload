# upload使用方法

upload支持较高版本的web（IE10+）和移动端浏览器
可参考demo文件夹中的使用

***

###  实例化
```
var up = new Upload({ ...参数 })
```

###  参数详情
| 参数名 | 注释 | 是否必填 | 格式/单位 | 返回值 |
| ---- | --- | --- | --- | --- |
| el | 容器,容器要设置宽高，上传插件依赖容器宽高| 是 | 传入#ID值或者dom |
| action |  上传表单的接口| 是 | string |
| data | 除了图片文件之外的参数 | 否 | object |
| multiple |  是否多选 | 否 | boolean |
| accept | 接受的文件类型，用于input本身的accept参数 | 否 | string |
| format | 接受的文件类型，用于上传的格式校验，值为文件的后缀名 | 否 | array |
| disabled |  是否禁用  | 否 | boolean |
| maxSize | 文件大小限制 | 否 | byte（单位） |
| formatError |  格式错误时的回调方法  |  错误的文件类型（遇到第一个错误就会终止），错误的文件数据 | 否 | function |
| oversize | 文件超过限制的回调方法  |  错误的文件类型（遇到第一个错误就会终止），错误的文件数据 | 否 | function |
| beforeUpload |  上传之前的方法  |  上传的文件列表 | 否 | function |
| success | 成功的回调  |  response | 否 | function |
| error |  错误的回调  |  response error | 否 | function |