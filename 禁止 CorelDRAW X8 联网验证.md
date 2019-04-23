# 禁止 CorelDRAW X8 联网验证

# Windows 防火墙
  控制面板\Windows防火墙\高级设置
 
    C:\Program Files\Corel\CorelDRAW Graphics Suite X8\Programs64\CorelDRW.exe
    C:\Program Files\Corel\CorelDRAW Graphics Suite X8\Programs64\DIM.exe
    C:\Program Files\Corel\CorelDRAW Graphics Suite X8\Programs64\CorelPP.exe
    C:\Program Files\Corel\CorelDRAW Graphics Suite X8\Draw\DIM.exe
  
  添加入站规则和出站规则，对上面4个程序设置阻止连接操作
  
# hosts
  C:\Windows\System32\drivers\etc\hosts
  
    127.0.0.1 apps.corel.com
    127.0.0.1 mc.corel.com
    127.0.0.1 origin-mc.corel.com
    127.0.0.1 iws.corel.com
  
  另起一行，添加上面内容,重启电脑或采取下面方法生效
  
    Win+R运行cmd
    输入  ipconfig /displaydns      #显示所有DNS
    输入  ipconfig /flushdns      #刷新所有DNS
    
    
