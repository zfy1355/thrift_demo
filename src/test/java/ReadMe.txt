
1.编写协议calculator.thrift
2.编译thrift文件
thrift-0.9.3.exe -r -gen java ./*.thrift
3.拷贝gen-java下生成的class类，到相应的目录下
4.
5.编写handler继承Iface，具体处理协议业务逻辑
6.生成ssl key :
	通过jdk/bin下的keytool工具：
	keytool -genkey -alias thrift -keyalg RSA
	生成.keystore存储在home目录下
7.python客户端安装 >pip install thrift

