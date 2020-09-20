<p align="center">
    <img alt="logo" src="https://raw.githubusercontent.com/fluentscheduler/FluentScheduler/version-6/Logo/logo-200x200.png">
</p>

Welcome to the documentation for FluentScheduler, an automated job scheduler with fluent interface for the .NET
platform.

```cs
JobManager.Initialize();

JobManager.AddJob(
    () => Console.WriteLine("5 minutes just passed."),
    s => s.ToRunEvery(5).Minutes()
);
```

Make sure to check the [GitHub repository](https://github.com/fluentscheduler/FluentScheduler) for community discussion
and its source code.
