
# QW-COMPOSE

## 目的

TODO

## 使用说明

TODO

### 创建网络 [^1]

TODO

### git使用

[ ] TODO

### portainer使用本repo

1. 登录 -> 点击`Stacks` -> 点击 `+ Add stack`
2. Name 自定义
3. Build method 选择 `Repository`
4. `Repository URL*`
    - 填入：`https://github.com/Qliangw/qw-compose`
5. Repository reference: `refs/heads/main`
6. Compose path: `buffet/xxx/docker-compose.yaml`
7. 导入环境变量：
    - 在 Environment variables 下找到 `advanced mode`
    - 在浏览器输入：`https://raw.githubusercontent.com/Qliangw/qw-compose/refs/heads/main/buffet/xxx/.env.example`

> 如果需要加速
> - `https://ghfast.top/https://github.com/Qliangw/qw-compose`
> - `https://ghfast.top/https://raw.githubusercontent.com/Qliangw/qw-compose/refs/heads/main/buffet/xxx/.env.example`

其中`buffet/xxx`中的xxx可以替换为buffet文件夹下的子目录名词

```shell
buffet
├── flare
├── moviepilot-v2
├── mtphotos
├── nginx-proxy-manager
└── vaultwarden
```

## 参考

[^1]: [自定义网络](https://docs.docker.com/reference/cli/docker/network/create/#specify-advanced-options)
[^2]: [使用外部已创建的网络](https://docs.docker.com/compose/how-tos/networking/#use-an-existing-network)
[^3]: [加入label](https://docs.docker.com/reference/cli/docker/compose/#use--p-to-specify-a-project-name)