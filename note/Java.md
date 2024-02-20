# Java
* mac os 配置idea maven: ->[跳转csdn](https://blog.csdn.net/weixin_43805744/article/details/128023702?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522170658296816800182153994%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=170658296816800182153994&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~baidu_landing_v2~default-6-128023702-null-null.142%5Ev99%5Epc_search_result_base9&utm_term=Mac%20设置maven&spm=1018.2226.3001.4187)

* wait和notify: ->[跳转csdn](https://blog.csdn.net/xhhhx_/article/details/124182042)

* mybatis: -> [跳转csdn](https://blog.csdn.net/vcj1009784814/article/details/106391982?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522170728639716800182724145%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=170728639716800182724145&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~top_positive~default-1-106391982-null-null.142%5Ev99%5Epc_search_result_base9&utm_term=mybatis&spm=1018.2226.3001.4187)

* 常量折叠：在编译过程中，Javac 编译器（下文中统称为编译器）会进行一个叫做 常量折叠(Constant Folding) 的代码优化。
            常量折叠会把常量表达式的值求出来作为常量嵌在最终生成的代码中，这是 Javac 编译器会对源代码做的极少量优化措施之一(代码优化几乎都在即时编译器中进行)。
            对于 String str3 = "str" + "ing"; 编译器会给你优化成 String str3 = "string"; 
            并不是所有的常量都会进行折叠，<mark>只有编译器在程序编译期就可以确定值的常量</mark>才可以：
            1. 基本数据类型( byte、boolean、short、char、int、float、long、double)以及字符串常量。
            2. final 修饰的基本数据类型和字符串变量
            3. 字符串通过 “+”拼接得到的字符串、基本数据类型之间算数运算（加减乘除）、基本数据类型的位运算（<<、>>、>>> ）
            <mark>引用的值在程序编译期是无法确定的，编译器无法对其进行优化。</mark>