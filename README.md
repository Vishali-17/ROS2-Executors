# Hello Guys 
Executors in ROS 2 are responsible for managing and executing callbacks in nodes.
A node can have multiple events such as topic subscriptions, services, and timers, which generate callbacks.
Instead of manually handling when and how each callback should run, the executor takes care of scheduling and execution.

## Two main types of executors:
SingleThreadedExecutor: Uses one thread, so only one callback runs at a time.
MultiThreadedExecutor: Uses multiple threads, allowing multiple callbacks to execute concurrently depending on system resources and callback group configuration.

In real life, a SingleThreadedExecutor is like a room with one door, where people must enter one by one.
A MultiThreadedExecutor is like a room with multiple doors, allowing multiple people to enter simultaneously.
