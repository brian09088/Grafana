# nssm 用來安裝服務:
- 移動到nssm目錄下啟動cmd(![image](https://github.com/brian09088/Grafana/assets/72643996/540c3707-90ea-4eb5-afc7-c686d28b8243)
```
nssm install loki
```
- 如果已經有安裝nssm會跳出視窗
- ![image](https://github.com/brian09088/Grafana/assets/72643996/8e58c555-1c69-40c7-bdb8-c7be3e7fb9a8)
- 其他如移除、啟動、暫停等指令，如下圖
- ![image](https://github.com/brian09088/Grafana/assets/72643996/c75e92b7-4572-44fd-b803-57e633be113d)

------
- loki
  - 透過移動執行目錄到loki資料夾下，啟動cmd
  ```
  .\loki-windows-amd64.exe --config.file=config.yaml
  ```
  - ![image](https://github.com/brian09088/Grafana/assets/72643996/5bc6b8e2-9887-4d1c-81d9-82e590efb37a)

- promtail(同上安裝程序，非必要套件)
- 目前已知問題:
  - 先啟動promtail再啟動loki，都成功啟動但是依然無法連接(localhost:3010 顯示404page not found，grafana則是Data source connected, but no labels received. Verify that Loki and Promtail is configured properly.)
  - ![image](/uploads/9cb5c70c888e0fb9d849abbf5fb2f817/image.png)
  - 先啟動loki再啟動promtail，出現錯誤
  - ![image](/uploads/53cd28e332bdf2cfbceb42a1b70e7ffe/image.png)
