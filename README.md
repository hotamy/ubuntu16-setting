# ubuntu16-setting
Ubuntu16.04 Setting note

## Bluetooth
  藍芽無線滑鼠無法使用，解決方式：
  
   `sudo vi /etc/bluetooth/main.conf`
  
  Change `#AutoEnable=false` to `AutoEnable=true`
  
   `sudo /etc/init.d/bluetooth restart`
  
  ## 安裝eclipse建立hyplink
  - 下載回來解壓縮後直接就可以執行（系統內已經裝好java了）
  
  - 解壓縮後把他移到 /opt 的目錄（這個是給第三方協力軟體放置的目錄）
  
    `sudo nautilus`（管理這身份開啟檔案總管）後移入
   
  - 建立捷徑hyplink
  
    `sudo gedit /usr/share/applications/eclipse.desktop`
  
    - 檔案內容
    ```
    [Desktop Entry]
    Name=Eclipse 4
    Type=Application
    Exec=/opt/eclipse/eclipse
    Terminal=false
    Icon=/opt/eclipse/icon.xpm
    Comment=Integrated Development Environment
    NoDisplay=false
    Categories=Development;IDE;
    Name[en]=Eclipse
    ```
