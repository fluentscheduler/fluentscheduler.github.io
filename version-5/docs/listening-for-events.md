To observe unhandled exceptions from your scheduled jobs listen for the JobException event on `JobManager`:

```cs
JobManager.JobException += info => Logger.Error("An error just happened with a scheduled job: " + info.Exception);
```

You can also listen for jobs start and end:

```cs
JobManager.JobStart += info => Logger.Information($"{info.Name}: started");
JobManager.JobEnd += info => Logger.Information($"{info.Name}: ended ({info.Duration})");
```
