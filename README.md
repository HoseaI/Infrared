# Infrared
通过HS0038B解码得到按键码

使用时先调用初始化函数，判断标志位再
获取键码
遥控器静音键键码为1 数字1键码为2 数字2键码为3
以此类推...
示例：extern uint8 irflag = 0;
      init_infrared();
      while(irflag)
      {
      irflag = 0;
      var = infrared_code();
      switch(var)
      {
       case 0 :     break;
       case 1 :     break;
       case 2 :     break;
       case 3 :     break;
        .....
      }
      }
