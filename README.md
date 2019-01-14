# Android
## 四大组件
### Activity
#### 四中启动模式及使用场景
#### Activity 生命周期
横竖屏切换的时候的生命周期
Activity 与 Fragment 之间生命周期比较
Activity 上有 Dialog 的时候按 Home 键的生命周期
前台切换到后台，然后再回到前台，Activity 生命周期回调方法
弹出 Dialog 生命周期回调方法
AlertDialog、PopupWindow、Activity 区别
下拉状态栏是不是影响 Activity 的生命周期
两个 Activity 之间跳转时必然会执行的是哪几个方法
如何保存 Activity 状态
Activity、View、Window 三者关系
Activity 之间的通信方式
Activity 启动过程
Fragment 生命周期
Fragment 状态保存 startActivityForResult 是哪个类的方法，什么情况下使用
如何实现 Fragment 的滑动
Fragment 之间传递数据的方式
Fragment 如果在 Adapter 中使用应该如何解耦

Service
生命周期
Activity 怎么和 Service 绑定
Service 和 Activity 怎么进行数据交互
Service 的开启方式
IntentService 原理及作用

ContentProvider
谈谈你对 ContentProvider 的理解
说说ContentProvider、ContentResolver、ContentObserver 之间的关系
ContentProvider 是如何实现数据共享的

广播
请描述对 BroadcastReceiver 的理解
广播的分类
广播使用方式和场景
静态注册与动态注册的区别
本地广播和全局广播有什么区别
如何通过广播拦截一条短信
广播是否可以请求网络
广播引起 ANR 的时间限制是多少

Context
谈谈对 Context 的理解
Application 和 Activity 的 Context 对象的区别

进程
进程间通讯的方式
Binder机制
进程等级
进程保活方案

性能优化
性能优化方案
内存优化
布局优化
网络优化
安装包优化

性能优化工具
如何对 Android 应用进行性能分析及优化
traceView 的使用
如何分析内存泄漏
启动页白屏及黑屏如何解决
启动太慢如何解决
怎样保证应用启动不卡顿
App 启动崩溃异常捕捉


动画
Android 中动画的分类
Android 动画框架实现原理

线程
Handler
Handler 机制
请解释下载单线程模型中 Message、Handler、Message Queue、Lopper 之间的关系
Handler、Thread、HandlerThread 的差别
Handler 发消息给子线程，Lopper 如何启动

AsyncTask
AsyncTask 原理
AsyncTask 的不足
如何取消 AsyncTask

子线程间如何通信
子线程与主线程间如何通信
为什么不能再子线程更新 UI
Android 线程有没有上限？
线程池有没有上限？
ThreadLocal 原理、实现及如何保证 Local 属性
服务器只提供数据接收接口，在多线程或多进程条件下，如何保证数据的有序到达？
CAS机制


图片加载与 Bitmap
LruCache、DiskLruCache 原理
LruCache 默认缓存大小
设计一个图片加载框架
如何避免 OOM
大图加载方案
Bitmap 对象的理解
Bitmap 使用时的注意事项
Bitmap 的 recycler()


View
事件分发机制
事件分发中的 onTouch 和 onTouchEvent 有什么区别
点击事件被拦截，但是想传到下面的 View 如何操作
绘制流程
UI 适配方案
LinearLayout、RelativeLayout、FrameLayout 的特性及对比
介绍下SurfaceView
RequestLayout、onLayout、onDraw、drawChild 区别与联系
invalidate 和 postInvalidate 的区别及使用
Activity、Window、View 三者的差别
如何优化自定义 View
自定义 View 如何考虑机型适配
如何计算一个 View 的嵌套层级
动态布局的理解


WebView
原生与 JS 交互的方式

SparseArray
SparseArray 原理

Java 虚拟机与 Dalvik/ART 虚拟机的区别

内存泄露与内存溢出
OOM 是什么
内存泄漏是什么
内存泄漏与内存溢出的关系
什么情况导致 OOM
什么方法能避免 OOM
什么情况导致内存泄漏
如何防止线程的内存泄漏

ANR 
ANR 产生的原因
ANR 定位和修正

适配
Android 各个版本 API 的区别
低版本 SDK 如何实现高版本 api
屏幕适配的处理技巧有哪些
动态权限适配方案，权限组的概念

架构设计
MVC、MVP、MVVM 的原理和区别

ListView 与 RecyclerView
ListView 的重用机制
RecyclerView 的使用
RecyclerView 的重用机制
RecyclerView 与 ListView 的区别
ListView 中图片错位问题如何产生的
ListView 优化
RecyclerView 优化

序列化
序列化的作用
Android 中两种序列化的区别
Android 为什么引入 Parcelable

网络
HttpUrlConnection 和 OkHttp 关系
HttpClient 与 HttpUrlConnection 的区别

ActivityThread、AMS、WMS 的工作原理

混合开发
知道的混合开发有哪些？优缺点和各自使用场景

插件化

三方库
OkHttp 优势

OkHttp 对比 Retrofit

OkHttp源码

Retrofit源码

RxJava源码
RxJava 的功能与原理实现

Glide 源码

Picasso Fresco Glide 对比

Java
Java 基础
final 的使用
static 的使用
String、StringBuffer、StringBuilder 的区别
谈谈对 Java 多态的理解
重载和重写的区别
Java 中 == 和 equals 和 hashCode 的区别
int、char、long 各占多少字节数
int 与 integer 的区别
什么是内部类？内部类的作用
抽象类和接口的区别
抽象类的意义
抽象类与接口的应用场景
抽象类是否可以没有方法和属性
接口的意义
泛型中 extends 和 super 的区别
父类的静态方法能否被子类重写
进程和线程的区别
final、finally、finalize 的区别
序列化的方式
Serializable 和 Parcelable 的区别
静态属性和静态方法是否可以被继承？是否可以被重写？原因
静态内部类的设计意图
成员内部类、静态内部类、局部内部类、匿名内部类的理解
String 转换成 Integer 的方式及原理
常见编码方式
utf-8 编码中中文占几个字节？int 几个字节？
静态代理和动态代理的区别，什么场景使用
Java的异常体系
修改对象 A 的 equals 方法的签名，那么使用 HashMap 存放这个对象实例的时候，会调用哪个 equals 方法？
如何将一个 Java 对象序列化到文件里
对 Java 反射的理解
对 Java 注解的理解
对依赖注入的理解
说一下泛型的原理并举例说明
String 为什么要设计成不可变的
为什么要将 Object 类的 equals 和 hashCode 方法重写？
Java 中对象的生命周期

JVM
GC机制
内存区域
内存模型
类记载过程
双亲委派模型
哪些情况下的对象会被垃圾回收机制处理掉

数据结构
并发集合了解哪些
列举 Java 的集合以及集合之间的继承关系
List、Set、Map 的区别
List 和 Map 的实现方式及存储方式
HashMap 的原理
HashMap 如何 put 数据
ConcurrentHashMap 的实现原理
ArrayMap 和 HashMap 的对比
HashTable 实现原理
TreeMap 实现原理
HashMap 和 HashTable 的区别
HashMap 和 HashSet 的区别
HashSet 和 HashMap 怎么判断集合元素重复
Set 怎么防止 Hash 碰撞
ArrayList 和 LinkedList 的区别及应用场景
数组和链表的区别
二叉树的深度优先遍历和广度优先遍历的具体实现
堆的结构
堆和树的区别
什么事深拷贝和浅拷贝
讲一下对树，B+树的理解
讲一下对图的理解
如何判断单链表是否成环


算法
快速排序
排序算法的区别
手写链表翻转代码
二叉树前、中、后序遍历
二叉树深度优先、广度优先遍历

多线程 
sleep 和 wait 的区别
join的用法
synchronized 的用法
synchronized 的原理
谈谈对类锁、方法锁、重入锁的理解
volatile 作用
volatile 和 synchronized 的区别
ReentrantLock、synchronized 和 volatile 比较
ReentrantLock 的内部实现
Lock 原理
死锁的四个必要条件
如何避免死锁
什么是线程池
线程间通讯
并发集合类
生产者和消费者模式
Thread 中的 start() 和 run() 方法有什么区别
开启线程的三种方式
线程和进程的区别
如何控制某个方法允许并发访问线程的个数
什么导致线程阻塞
线程如何关闭
Java 中的同步方法
如何保证数据一致性
如何实现线程同步
两个线程同时要求写或者读能否实现？
线程间操作 List


设计模式
知道的设计模式有哪些
项目中常用的设计模式
手写生产者/消费者模式
适配器模式、装饰者模式、外观模式的异同
手写单例模式

引用类型的区别与使用场景

异常处理
Exception 和 Error 的区别
网络
http、https
TCP 三次握手流程
TCP 和 UDP 的区别
Socket 建立网络连接的步骤