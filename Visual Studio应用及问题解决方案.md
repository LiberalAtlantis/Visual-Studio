# Visual Studio应用及问题解决

## 1 应用

Visual Studio 2022 官方支持文档

[https://docs.microsoft.com/zh-cn/visualstudio/install/install-visual-studio?view=vs-2022]

扩展工具下载

[https://www.nuget.org/]

扩展包下载

[https://www.nuget.org/packages]

扩展工具使用文档

[https://docs.microsoft.com/en-us/nuget/]

C# 教程

[https://docs.microsoft.com/zh-cn/dotnet/csharp/]

[https://docs.microsoft.com/zh-cn/dotnet/]

控件及控件属性

[https://docs.microsoft.com/zh-cn/dotnet/desktop/wpf/controls/?view=netframeworkdesktop-4.8]

## 2 扩展

## 3 问题及解决措施

### 3.1 Visual Studio 2022 兼容性问题

#### 3.1.1 不支持 .NET Framework 4.5

##### 3.1.1.1 问题

默认Visual Studio 2022 不再支持安装 .NET Framework 4.5 组件，选择组件里面已经不能选择 4.5/4.0 的框架。

如果打开基于 .NET Framework 4.5 的项目会收到提示：

（1）将目标更新为 .NET Framework 4.5 目标包。

（2）下载 .NET Framework 4.5 目标包。

（3）请勿加载此项目。

##### 3.1.1.2 解决措施

（1）nuget 下载 4.5 安装包

下载地址：[https://www.nuget.org/packages/microsoft.netframework.referenceassemblies.net45]

（2）将文件复制到系统目录

以 zip 方式解压下载的安装包.nupkg（可以直接修改后缀名为 .zip 再进行解压）

复制：build\.NETFramework\v4.5\ 到 C:\Program Files (x86)\Reference Assemblies\Microsoft\Framework\.NETFramework\v4.5

（3）重启 Visual Studio 2022
