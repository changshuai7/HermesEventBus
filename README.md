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

1、修复ActionBarActivity找不到的错误(xiaofei.library.hermes.util.TypeUtils)


原项目地址：

1、[HermesEventBus](https://github.com/Xiaofei-it/HermesEventBus)

2、[Hermes](https://github.com/Xiaofei-it/Hermes)

3、[Concurrent-Utils](https://github.com/Xiaofei-it/Concurrent-Utils)

[文档请点击](doc)

混淆配置：

	-keep class evbean.** { *; }  #这里写你自己的javabean
	#EventBus
	-keepattributes *Annotation*
	-keepclassmembers class ** {
	    @org.greenrobot.eventbus.Subscribe <methods>;
	}
	-keep enum org.greenrobot.eventbus.ThreadMode { *; }
	# Only required if you use AsyncExecutor
	-keepclassmembers class * extends org.greenrobot.eventbus.util.ThrowableFailureEvent {
	    <init>(java.lang.Throwable);
	}
	-keep class xiaofei.** { *;}
	-dontwarn xiaofei.** 

