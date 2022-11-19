# Linux_learn_boot_analyze
系統重啟時間分析

參考 : 

* [Time it takes to reboot a Linux server](https://unix.stackexchange.com/questions/274339/time-it-takes-to-reboot-a-linux-server)

* [Is there a way to see the execution tree of systemd?](https://serverfault.com/questions/617398/is-there-a-way-to-see-the-execution-tree-of-systemd)

systemd-analyze ( 大略需要時間 )
---

```
啟動 systemd 後上次啟動花費了多少時間。
這沒有考慮 BIOS/硬件初始化或 GRUB 超時，
但對於實際的操作系統啟動時間應該是準確的
```

![image](https://user-images.githubusercontent.com/96226780/202847517-f69aecc7-8a11-43aa-9301-2f96c81e64cc.png)

systemd-analyze blame ( 解析 )
---

![image](https://user-images.githubusercontent.com/96226780/202847523-50f24c07-3477-4532-8ec2-0f64d4808baf.png)
