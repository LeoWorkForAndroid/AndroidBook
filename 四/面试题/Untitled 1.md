### IntentService和Service

```
生成一个默认的且与主线程互相独立的工作者线程来执行所有传送至onStartCommand() 方法的Intetnt。

生成一个工作队列来传送Intent对象给你的onHandleIntent()方法，同一时刻只传送一个Intent对象，这样一来，你就不必担心多线程的问题。在所有的请求(Intent)都被执行完以后会自动停止服务，所以，你不需要自己去调用stopSelf()方法来停止。

该服务提供了一个onBind()方法的默认实现，它返回null

提供了一个onStartCommand()方法的默认实现，它将Intent先传送至工作队列，然后从工作队列中每次取出一个传送至onHandleIntent()方法，在该方法中对Intent对相应的处理。

多次启动IntentService，IntentService是等前面的请求结束之后再执行下一个。 这个证实了 IntentService 采用单独的线程每次只从队列中拿出一个请求进行处理


这就是IntentService，一个方便我们处理业务流程的类，它是一个Service，但是比Service更智能。

```

