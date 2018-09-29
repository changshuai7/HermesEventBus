# HermesEventBus
HermesEventBus跨进程通信框架

Step 1：Add it in your root build.gradle at the end of repositories:

	allprojects {
		repositories {
			...
			maven { url 'https://www.jitpack.io' }
		}
	}

Step 2. Add the dependency

	dependencies {
	        implementation 'com.github.changshuai7:HermesEventBus:1.0.0'
	}

本项目基于原项目(2018.09.29-->HermesEventBus0.3.0/Hermes0.7.0/Concurrent-Utils0.1.4)
修改了如下：
1.修复ActionBarActivity找不到的错误


原项目地址：
[HermesEventBus](https://github.com/Xiaofei-it/HermesEventBus)

[Hermes](https://github.com/Xiaofei-it/Hermes)

[Concurrent-Utils](https://github.com/Xiaofei-it/Concurrent-Utils)

[文档请参照](doc)
