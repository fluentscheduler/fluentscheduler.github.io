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
