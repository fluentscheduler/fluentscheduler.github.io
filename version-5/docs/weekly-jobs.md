Let's suppose it's 10:00 of a Monday morning and you want to start a job that runs every Monday at 14:00.
Should the first run of your job be today or only on the next week Monday?

If you want the former (not waiting for a whole week):

```cs
// Every "zero" weeks
Schedule<MyJob>().ToRunEvery(0).Weeks().On(DayOfWeek.Monday).At(14, 0);
```

Or if you want the latter (making sure that at least one week has passed):

```cs
// Every "one" weeks
Schedule<MyJob>().ToRunEvery(1).Weeks().On(DayOfWeek.Monday).At(14, 0);
```
