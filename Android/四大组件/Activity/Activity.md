## 四大组件

## Activity

### Activity 的四种启动模式及使用场景

- standard

  标准模式，Activity 的默认启动模式。每次启动一个 Activity 时都会创建一个新 Activity 的实例并放入任务栈中。

  使用场景：一般场景都可以。

- singleTop

  栈顶复用模式。当在此模式下新建一个 Activity，如果任务栈的栈顶已存在该 Activity 的实例，那么将不会再创建该 Activity 的实例，同时会调用 onNewIntent(Intent intent) 方法，在方法参数 intent 中可以取出当前请求的信息，并且 onCreate、onStart 方法不会被调用。

  使用场景：用于登录、用户信息等一些不希望因重复点击出现多个的页面。

- singleTask

  栈内复用模式。当在此模式下新建一个 Activity，如果任务栈中已经存在该 Activity 的实例，那么将不会再创建该 Activity 的实例，同时会将栈中该 Activity 实例上面所有 Activity 使用移除将其置于栈顶，并调用 onNewIntent(Intent intent) 方法，在方法参数 intent 中可以取出当前请求的信息。

  使用场景：主页面

- singleInstance

  单实例模式。当在此模式下新建一个 Activity，会创建一个该 Activity 的实例并放置在一个单独的新的任务栈。并且由于栈内复用机制，如果栈中已存在该 Activity 实例则不会再创建该 Activity 的实例，并且会调用 onNewIntent(Intent intent) 方法。

  使用场景：Android 系统的电话页面等多应用共享页面。

### 如何设置 Activity 的启动模式

- 通过 AndroidManifests 文件

  ```java
  <activity
  	android:name=".MainActivity"
  	android:launchMode="singleTask" />
  ```

- 通过 Intent 设置标志位，优先级高于 AndroidManifests

  ```java
  Intent intent = new Intent(this, MainActivity.class);
  intent.addFlags(Intent.FLAG_ACTIVITY_SINGLE_TOP);
  startActivity(intent);
  ```

### 常用标记位

- FLAG_ACTIVITY_NEW_TASK

  作用等同于 singleTask

- FLAG_ACTIVITY_SINGLE_TOP

  作用等同于 singleTop

- FLAG_ACTIVITY_CLEAR_TOP

  一般配合 FLAG_ACTIVITY_NEW_TASK 使用，效果类似于 singleTask