# upload使用方法

upload支持较高版本的web（IE10+）或移动端浏览器

***

###实例化
`var up = new Upload({ ...参数 })`

###参数详情
参数名 | 注释 | 返回值
---- | --- | ---
el | 容器名称，传入#ID值或者dom（容器要设置宽高，上传插件依赖容器宽高）
action |  上传表单的接口，必填
data | 除了图片文件之外的参数
multiple |  是否多选
accept | 接受的文件类型
disabled |  是否禁用
maxSize | 文件大小限制，单位为 byte
formatError |  格式错误时的回调方法  |  错误的文件类型（遇到第一个错误就会终止），错误的文件数据
oversize | 文件超过限制的回调方法  |  错误的文件类型（遇到第一个错误就会终止），错误的文件数据
beforeUpload |  上传之前的方法  |  上传的文件列表
success | 成功的回调  |  response
error |  错误的回调  |  response error