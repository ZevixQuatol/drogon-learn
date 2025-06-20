# drogon-learn
    从零开始drogon学习
    我的开发环境
    平台：      windows
    编辑器：    clion
    编译器：    minGW
    构建：      cmake
    包管理：    vcpkg
# 1. cmake
    跳过安装 环境变量配置
# 2. minGW
    跳过安装 环境变量配置
# 3. vcpkg
## 环境变量配置
    path: vcpkg安装目录
### 3.1 指定安装目录
    VCPKG_INSTALLATION_ROOT=文件夹
### 3.2 配置minWG编译
    VCPKG_DEFAULT_TRIPLET=x64-mingw-dynamic
    VCPKG_DEFAULT_HOST_TRIPLET=x64-mingw-dynamic
# 4. drogon
## 安装
    vcpkg install jsoncpp:x64-mingw-dynamic zlib:x64-mingw-dynamic openssl:x64-mingw-dynamic sqlite3:x64-mingw-dynamic libpq:x64-mingw-dynamic libpqxx:x64-mingw-dynamic drogon[core,ctl,sqlite3,postgres,orm,redis]:x64-mingw-dynamic
## 引入
    //配置环境变量
    VCPKG_INSTALLATION_ROOT\x64-mingw-dynamic\tools\drogon
    VCPKG_INSTALLATION_ROOT\x64-mingw-dynamic\bin
    VCPKG_INSTALLATION_ROOT\x64-mingw-dynamic\lib
    VCPKG_INSTALLATION_ROOT\x64-mingw-dynamic\include
## 检查
    1. 重启cmd
    2. 输入drogon_ctl 或 drogon_ctl.exe 出现以下内容：

    usage: drogon_ctl [-v | --version] [-h | --help] <command> [<args>]
    commands list:
    create                  create some source files(Use 'drogon_ctl help create' for more information)
    help                    display this message
    press                   Do stress testing(Use 'drogon_ctl help press' for more information)
    version                 display version of this tool
