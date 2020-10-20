### Kail攻擊
```
1.如何找到受害者的系統漏洞

  用Nmap找該ip的系統
  Ep. nmap --script=valn 10.0.2.4 
  
2.如何找到受害者MAC 地址
  可以用netdiscover掃描受害者的IP 然後從而找到相對的MAC地址
  
```

### 防禦
```
1.可以用cmd中的netstat來找出可疑連接
  Ep.netstat -ano 
   netstat -a 可以找到所有活動的TCP連接、ip位址、狀態，但是無法查看PID
           -n 只可以找到活動中的連接，而且不能查看PID
