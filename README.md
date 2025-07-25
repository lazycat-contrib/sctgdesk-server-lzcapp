# sctgdesk-server-lzcapp
## 使用说明
### Key
key需要通过懒猫开发者工具获取
### 网络映射
如果家庭宽带有公网ip,转发21114-21119到设备ip即可.其中21116端口既要开放tcp也要开放udp
端口说明

- `hbbs`:

  - `21114` (TCP): used for web console, only available in `Pro` version.
  - `21115` (TCP): used for the NAT type test.
  - `21116` (TCP/UDP): **Please note that** **`21116`** **should be enabled both for TCP and UDP.**  `21116/UDP` is used for the ID registration and heartbeat service. `21116/TCP` is used for TCP hole punching and connection service.
  - `21118` (TCP): used to support web clients.
- `hbbr`:

  - `21117` (TCP): used for the Relay services.
  - `21119` (TCP): used to support web client
