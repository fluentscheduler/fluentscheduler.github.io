<p><strong>Important: this documentation refers to the version 5 of the library which is currently deprecated. Check the current version <a href="https://fluentscheduler.github.io">here</a>.</strong></p>
<hr>

By default, the library allows a schedule to run in parallel with a previously triggered execution of the same
schedule.

If you don't want such behaviour you can set a specific schedule as non-reentrant:

```cs
public class MyRegistry : Registry
{
    Schedule<MyJob>().NonReentrant().ToRunEvery(2).Seconds();
}
```

Or you can set it to all schedules of the registry at once:

```cs
public class MyRegistry : Registry
{
    NonReentrantAsDefault();
    Schedule<MyJob>().ToRunEvery(2).Seconds();
}
```
