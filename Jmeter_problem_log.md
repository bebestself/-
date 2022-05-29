### Jmeter发送的请求响应内容乱码：
- 方法1：使用后置处理器-BeanShell 后置处理程序，配置为：`prev.setDataEncoding("utf-8")`
- 方法2：修改jmeter/bin/jmeter.properties文件，查找"sampleresult.default.encoding"修改编码为：utf-8，并去掉注释，保存后重启jmeter
