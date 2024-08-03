# makerbase-mks-dlc32-web-commands

[]

[![Watch the video]([https://img.youtube.com/vi/OY3z75zqwP8/hqdefault.jpg](https://user-images.githubusercontent.com/12979070/131437599-2b7aae8f-1569-4e38-b713-bb6b87596be5.png))](https://www.youtube.com/embed/OY3z75zqwP8)

[!https://user-images.githubusercontent.com/12979070/131437599-2b7aae8f-1569-4e38-b713-bb6b87596be5.png]

If upload probe.html in same folder with index.html.gz (mks-about-update webui-select files-upload probe.html)

And open http://ip-mks/probe.html

Bellow some utils web commands to comunicate with mks dlkc32:

       http://www.msftconnecttest.com/command?commandText=$J=G91%20G21%20F1500%20X-50&PAGEID=0 ----- move axe x 50

       http://www.msftconnecttest.com/command?commandText=$J=G91 G21 F1500 X50 ----- move axe x 50

       http://www.msftconnecttest.com/command?commandText=M3 S10 (M3-pwm on S10-Set power 10) 
       
       http://www.msftconnecttest.com/command?commandText=M5 (M5-pwm off)

       http://www.msftconnecttest.com/command?commandText=%5BESP220%5D/Agata.nc&PAGEID=0 (execute Agata.nc from sd card)

       http://www.msftconnecttest.com/command?commandText=%5BESP221%5D/Agata.nc&PAGEID=0 (list Agata.nc gcode)

       http://www.msftconnecttest.com/upload?path=%2F&action=delete&filename=Alex.nc&PAGEID=0 (delete Alex.nc from sd card)

       http://www.msftconnecttest.com/files (quando salvo index.html.gz)

       http://www.msftconnecttest.com/files?action=list&filename=all&path=/&PAGEID=1



https://github.com/makerbase-mks/MKS-DLC32/tree/main/MKS-DLC32-main/firmware

 https://github.com/makerbase-mks/MKS-DLC32/blob/main/MKS-DLC32-main/firmware/tool/MKSLaserTool_setupV2.0.4.rar

       MKS-DLC32-FIRMWARE-main\Firmware\Grbl_Esp32\src\WebUI\WebServer.cpp  line 149
       _webserver->on("/command", HTTP_ANY, handle_web_command);
        _webserver->on("/command_silent", HTTP_ANY, handle_web_command_silent);
