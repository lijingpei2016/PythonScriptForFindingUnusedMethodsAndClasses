# PythonScriptForFindingUnusedMethodsAndClasses
查找无用类和方法的pythone脚本（2023年）

1.修改了文件路径

2.简单的工程方法列表是在__DATA_CONST，而非__DATA
lines = os.popen('/usr/bin/otool -v -s __DATA_CONST __objc_classlist %s' % path).readlines()
lines = os.popen('/usr/bin/otool -v -s __DATA __objc_classlist %s' % path).readlines()

