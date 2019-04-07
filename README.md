# Activitylife
验证Activity的生命周期
Activity的状态可分为四种：运行状态、暂停状态、停止状态、销毁状态。

  在Activity的生命周期中，有七种方法会被系统回调：

onCreat（）；onStart（）；onRestart（）；onResume（）；onPause（）；onStop（）；onDestroy（）。

  运行状态：当前Activity位于前台，用户可见，可直接操作，即是我们正在使用当前的Activity；

  暂停状态：当前Activity位于前台，用户可见，但不可直接操作，也就是我们在打开了Activity之后又运行了另一个Activity，
  这时，前一个Activity就处于暂停状态，而正在运行的Activity就是运行状态。

  停止状态:该状态下，Activity退出前台，为不可见的状态，当Activity处于前台时，我们按下显示主屏幕键，此时Activity
  就退出前台，这时就是处于停止状态。在停止状态时，我们返回到这个Activity，系统回调onRestart方法，重新让Activity回到运行状态，并回调onStart方法。

  关闭状态：当Activity从停止状态退出后台时，Activity就被关闭，此时无法在调用方法使其回到其他状态，
  到此Activity的一个生命周期就结束了，只有重启才能开始下一个生命周期。
测试Activity的生命周期可以通过重写父类的方法，设置log日志，在调试的时候能够通过日志，看到Activity的状态。
以下为测试截图：
![Image text](https://raw.githubusercontent.com/695400861/Activitylife/master/image/2%7DV%60X94%7DL%7B%40NDVNLH%25VXK_W.png)

![Image text](https://raw.githubusercontent.com/695400861/Activitylife/master/image/%5DT65YF8~LB(DX8%24%60%25%5D%40GFZT.png)




