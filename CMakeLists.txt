

#项目名称 Main
project (Main)

#自动将当前目录下的文件 .c .h .cpp 打包在一个变量中
aux_source_directory("." DIR_SRC)


#添加可执行文件  可执行文件名称
#将文件 编译成 Main的可执行文件
#add_executable(Main "main.cpp")

#全部 将保存的变量添加上去
add_executable(Main ${DIR_SRC})