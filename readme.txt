编译指令
1。安装Arduino IDE
你可以在这里获得最新的Arduino IDE:
http://arduino.cc/en/Main/Software
Atmel AVR主板至少需要1.0版本，ARM主板至少需要1.5版本。
2。确保安装了打印机板的串行驱动程序。Arduino IDE包含签名驱动程序
Arduino的电路板取决于你的董事会，你可能需要不同的驱动器，然后这些。适用于Linux和Mac
你通常不需要任何额外的驱动程序。询问您的打印机/板供应商您需要哪种驱动程序，
如果你不清楚的话。
3所示。一些不是原始arduino板，并不是100%兼容，需要单独的扩展
Arduino IDE安装它们。
4所示。启动Arduino IDE，打开文件“Repetier.ino”
5。在arduino ide中选择要上传的板和端口。
6。如果需要检查或修改某些内容，请检查Configuration.h以获得提示。
7所示。用上传按钮(工具栏上的右箭头)上传固件。
如果你有一个正常的mega 2560兼容板，你可以使用arduino的代码块而不是arduino ide:
http://arduinodev.com/codeblocks/
打开Repetier。CBP文件而不是ino文件，并从6开始。
提示:如果您启用了eeprom支持，第一次上传将把配置复制到eeprom中。晚些时候
上传不会覆盖这些设置!与重复主机连接到您的打印机，并打开eeprom编辑器
更改这些值。或者，发送命令
M502
M500
将Configuration.h中的新值复制到eeprom。
对用户很重要
还有一个附加的文件夹AdditionalArduinoFiles，它带有单独的自述文件，描述了如何获取
监督工作。用工作的看门狗来编译是一个非常好的想法!!