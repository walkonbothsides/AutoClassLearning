
## 使用方法

1. 首先需要在运行设备上安装Python3运行环境。具体安装方法可以参考网上的教程进行一般操作。或者也可以使用包管理器很方便安装Python（Windows用户可以使用Choco，Mac可以使用Brew，Linux用户，恩，包管理器对于Linux用户来说就是传统艺能）。如果遇到库导入错误，请检查您的Python版本，务必为3

2. 接着打开命令行操作界面，CD（Change Directory）到该脚本的目录下

3. 最后执行`python main.py` 或者 `python3 main.py`即可开始运行该脚本，按照指示使用即可。

## 可以自定义的地方

1. 院校码，这个没有深入研究如何获取到具体学校的tenantCode(院校码，用于发送请求时区分学校)。每个学校的都是不同的，如果你想获取自己学校的tenantCode的话，你可以自己试着登录一次，在浏览器开发者工具中的网络选项卡中查看网络请求信息抓取。或者实在不会操作可以提个Issues过来。（现已加入TODO，该信息可以在登录页面中请求到一个巨大的JSON）

2. 课程间的延迟时间，在**WeiBanAPI.py文件**的头部中有两个参数分别为**baseDelayTime**基础延时秒数和**randomDelayDeviation**叠加随机延时差。**实际延迟时间 = 基础延时秒数 + 叠加随机延时差**
