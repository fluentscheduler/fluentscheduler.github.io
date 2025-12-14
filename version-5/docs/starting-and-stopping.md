<p><strong>Important: this documentation refers to the version 5 of the library which is currently deprecated. Check the current version <a href="https://fluentscheduler.github.io">here</a>.</strong></p>
<hr>

With the [registry](creating-schedules.md) ready, you then need to initialize the `JobManager`:

```cs
JobManager.Initialize(myRegistry);
```

To stop the scheduler:

```cs
JobManager.Stop();
```

To both stop and wait for the running jobs to finish:

```cs
JobManager.StopAndBlock();
```
