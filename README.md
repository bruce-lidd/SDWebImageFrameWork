# SDWebImageFrameWork
SDWebImage类库制作
首先介绍一下什么是framework：
framework是资源的集合，将静态库（ios8以后可以是动态库）和其头文件包含到一个结构中，让XCode可以方便的把它纳入到你的项目中。
分为真机－Debug（调试）版本、真机－Release（发布）版本、模拟器－Debug版本、模拟器－Release版本；开发中一般都打包Release（发布版本），将真机和模拟器合并，提供给外界。
在项目开发过程中，例如两个公司之间业务交流，不可能把源代码都发送给另外一个公司，这时候将私密的内容打包成framework，别人只能调用接口，而不能知道其中实现的细节。
framework对CPU架构的支持，首先了解ios设备cpu架构方面的知识，ARM是微处理器行业的一家知名企业，ARM处理器以体积小和高性能的优势在嵌入式设备中广泛使用，几乎所有的手机都是使用他的：
模拟器：iphone4s－5:i386， iphone5s－6splus：x86——64
真机：iphone3gs－4s：armv7， iphone5-5c：armv7s iphone5s－6splus：arm64
armv7、armv7s是ARM CPU的不同指令集，原则是向下兼容的，例如iphone4sCPU支持armv7，但它同时兼容armv6，只是使用armv6指令可能无法充分发挥它的特性。
