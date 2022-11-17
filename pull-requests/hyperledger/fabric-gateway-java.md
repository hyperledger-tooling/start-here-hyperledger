---
layout: default
title: fabric-gateway-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway-java
---

# fabric-gateway-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway-java/pull/124" class=".btn">#124</a>
            </td>
            <td>
                <b>
                    Add the ability to config HFClient executorService through Gateway to Solve OutOfMemoryError
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                when receiving event block, Channel class call 
`HFClient.getExecutorService.execute(() -> l.listener.received(blockEvent))`

If HFClient executorService is not set, HFClient use the default executorService which is [ThreadPoolExecutor](https://docs.oracle.com/javase/8/docs/api/index.html) with **Direct handoffs strategy** for queuing that strategy hands off tasks to threads without otherwise holding them. it's create new native Thread to run task if if no threads are available to run it.

HFClient default executerServise(ThreadPoolExecutor) has the following properties:
- corePoolSize = 0
- maximumPoolSize = Integer.Max(2147483647)
- keepAliveTime = 60
- timeUnit = SECONDS
- workQueue = SynchronousQueue (that hands off tasks to threads without otherwise holding them. 
		an attempt to queue a task will fail if no threads are immediately available to run it(require unbounded maximumPoolSizes to avoid rejection of new submitted tasks), so a new thread will be constructed)
- threadFactory = create new thread using Executors.defaultThreadFactory()


If the program receives a huge number of block events at the same time,it creates new **native Thread which is expensive resource** for every task to handle block event. this maybe cause 
```
java.lang.OutOfMemoryError: unable to create new native thread
	at java.lang.Thread.start0(Native Method)
	at java.lang.Thread.start(Thread.java:717)
	at java.util.concurrent.ThreadPoolExecutor.addWorker(ThreadPoolExecutor.java:957)
	at java.util.concurrent.ThreadPoolExecutor.execute(ThreadPoolExecutor.java:1378)
	at org.hyperledger.fabric.sdk.Channel.lambda$startEventQue$13(Channel.java:5954)
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1149)
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:624)
	at java.lang.Thread.run(Thread.java:748)
```
depend on machine resouces. 

so we need way to custmize HFClient executerServise through Gateway.Builder, 
The new method:
`Builder clientExecutor(ExecutorService executorService);` 
was added to Gateway.Builder to give the freedom to the library user to use another executerServise with anothor queuing strategies 
like **Unbounded queues Strategy** or Bounded queues strategy to **actually enqueue Tasks**.

### How to use
```
ThreadPoolExecutor executor = new ThreadPoolExecutor(corePoolSize, maximumPoolSize,
				0, TimeUnit.MILLISECONDS, new LinkedBlockingQueue<>(),
				r -> {
					Thread thread = defaultThreadFactory().newThread(r);
					thread.setDaemon(true);
					return thread;
				});
Builder builder = Gateway.createBuilder();
builder.identity(wallet, orgMSPName).networkConfig(networkConfigPath).discovery(true)
	.executorService(executor).commitHandler(DefaultCommitHandlers.NONE);
gateway = builder.connect();
```

with the added changes and the executorService above with **Unbounded queues Strategy**, Program was able hadle Tens of thousands of block events received at the same time steadily withot facing annoying OutOfMemoryError and without need to upgrade machines. because **storing tasks in Queue consumes mush less memory than creating native Threads**. in addition to avoid Context Switching.

closes #84 
may also ratated to issue #106 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-16 23:59:54 +0000 UTC
    </div>
</div>

