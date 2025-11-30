# DDMC-AUTO
针对特定电商平台数据流转需求，使用Qt C++开发的一款集成自动化操作的桌面端软件。  

工作流程：  

1.通过系统API调取本机的机器码以及MAC地址，与数据库进行比对，完成之后即可登陆客户端  

2.登陆过后有多项功能供使用：  

  a.主功能，读取售后软件售后信息，进行售后筛选，记录联系方式，申请时间，售后种类，可选定售后类型进行筛选与发送  
  
    筛选完成后模拟鼠标点击使用微信或者其他平台进行发送，实现远程处理售后，无需长时间盯盘（本想使用微信API,由于封号严重并未采取此方案）  
    
  b.自动选取常用售后类型进行筛选  
  
以下是客户端的部分ui界面
<img width="2880" height="1800" alt="image" src="https://github.com/user-attachments/assets/209c89ce-c7ca-4278-b91d-caa4ce040e17" />

以下是客户端部分代码
<img width="2880" height="1800" alt="image" src="https://github.com/user-attachments/assets/02f6fa59-1674-4d89-b6dc-3b8e10d19b94" />

以下是用来操作存储客户机器码以及MAC地址的部分ui,用户在购买后客户端会自动获取机器码和MAC地址，获得机器码和MAC地址后即可通过此系统传入验证服务器的mysql数据库。
<img width="2877/2" height="1800" alt="image/2" src="https://github.com/user-attachments/assets/e79c2d93-454e-4c5a-b791-7ba8f1c0b6be" />

以下是操作数据库的部分代码
<img width="2880/2" height="1800/2" alt="image" src="https://github.com/user-attachments/assets/10a79cd3-2f50-4aab-b50c-b1bb3b5700ea" />
