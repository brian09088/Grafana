# 用來安裝服務:
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
