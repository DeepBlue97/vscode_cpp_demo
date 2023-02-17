project(test) # 项目名称

# set(LANGUAGE CXX)
aux_source_directory(./src SRCS)  # 所有SRCS字样会被源文件名替换掉。

add_executable(${PROJECT_NAME} ${SRCS})  # 可执行文件名 设置为 项目名
# 效果同
# add_executable(test ./src/hello.cpp ./src/test.cpp)