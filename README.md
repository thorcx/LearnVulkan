
##配置方法
* 1.编辑RunFromVsCode.bat,在文件内指定了vcvars64.bat的位置，编辑为你自己机器上的位置
* 2.运行RunFromVsCode.bat,如果已经装好了vscode，编辑器会自动打开并定位到当前程序
* 3.在.vscode内的tasks.json文件内定义了编译器cl的编译选项，包括链接vulkan库与glfw库
* 4.c_cpp_properties.json定义了intellsense的头文件包含规则，注意这里设置完并不能实际编译就引用，必须在编译选项指定/I路径
* 5.launch.json定义了Debugger