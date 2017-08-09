服务器端自动启动shadowsocks：
复制 `ssserver.service` 放到 `/lib/systemd/system/` 目录下，然后运行:

    sudo systemctl daemon-reload
    sudo systemctl enable ssserver
    sudo systemctl start ssserver
    sudo systemctl status ssserver

 MacOS自动启动:
 Shadowsocks,将`shadowsocks.plist`放到`~/Library/LaunchAgents/`目录下： 然后运行

     launchctl load -w shadowsocks.plist
     
  然后重启macbook即可自动启动shadowsocks了
