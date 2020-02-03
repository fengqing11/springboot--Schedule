# springboot定时任务--@Scheduled

## 遇到的问题：

1.Caused by: java.lang.IllegalStateException: Encountered invalid @Scheduled method 'cron': Cron expression must consist of 6 fields (found 1 in "0****?")

解决办法：cron = "0 * * * * ?"表示每分钟都执行一次。（注意中间有空格。不然会报错）

