# lunar
python公历转农历  
特点：  
1、封装成类，直接调用。  
2、返回数据多样，可返回农历数据元祖如返回：（2023,11,14）或农历汉字文本（不含年）如返回：正月初一   
3、未使用第三方库，都是python自带库，可以直接在micropython上运行。    
4、调用举例：  
  from LUNAR import LUNAR  
  y,m,d = 2023, 11, 14 #国历  
  lunar=LUNAR()  
  print(lunar.get(y,m,d)) #返回元祖  
  print(lunar.getChinese(y,m,d)) #返回汉字文本  
