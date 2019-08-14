# Java多线程

- ## Java实现多线程有哪几种方式

  继承Thread类，实现Runnable接口，实现Callable接口。

- ## 线程池的参数有哪些，在线程池创建一个线程的过程
  
        ThreadPoolExecutor(
            int corePoolSize, // 核心线程数量
            int maxPoolSize,  // 最大线程数
            long timeTolive, // 线程存活时间
            TimeUnit timeUnit, // 存活时间单位
            BlockingQueue<Runnable> queue, // 任务队列
            RejectExecutionHandler rejectHandler // 拒绝策略
        )