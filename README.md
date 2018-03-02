# ubuntu16-setting
Ubuntu14.04 Setting note

## Bluetooth
  藍芽無線滑鼠無法使用，解決方式：
  
  `sudo vi /etc/bluetooth/main.conf`
  
  Change `#AutoEnable=false` to `AutoEnable=true`
  
  `sudo /etc/init.d/bluetooth restart`
