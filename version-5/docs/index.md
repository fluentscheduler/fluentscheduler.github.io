<p align="center">
    <img alt="logo" src="https://raw.githubusercontent.com/fluentscheduler/FluentScheduler/version-6/Logo/logo-200x200.png">
</p>

<p><strong>Important: this documentation refers to the version 5 of the library which is currently deprecated. Check the current version <a href="https://fluentscheduler.github.io">here</a>.</strong></p>
<hr>

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
