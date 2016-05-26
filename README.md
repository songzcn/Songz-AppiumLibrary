# SongzAppiumLibrary
对robotframework-appiumlibrary进行了补充，增加了以下关键字<br />
# 安装方法
下载到python27\Lib\site-packages目录下，更改文件夹名为SongzAppiumLibrary。使用时导入SongzAppiumLibrary，不再导入AppiumLibrary<br />
<br />
# current activity 
返回当前activity名<br />
# wait activity       
参数：activity timeout interval<br />  
在超时时间内获取到目标activity,返回True,否则返回False<br />
# start activity 
参数：package activity **opts(可选，参照f5)    
启动指定进程（可跨应用），类似于switch application关键字，更贴近python-appium使用习惯<br />
# open notifications                         
打开系统通知栏（api>=19）<br />
# available ime engines                          
返回系统所有可用的输入法<br />
# is ime active                               
检查当前设备是否有输入法服务，有的话返回True,否则返回False<br />
# activate ime engine    
参数：engine                  
激活指定的输入法（设备须预安装该输入法）<br />
# deactivate ime engine     
恢复当前设备的输入法服务<br />
# click element after find it      
参数：locator        
点击长列表中任意可点的元素，ios（tableview）、安卓(listview)通用<br />
# swipe percentage      
参数：p1 p2 p3 p4(arguments like 0.5,0.75,0.435) duration       
按比率划屏<br />
<br />
# swipe element percentage      
参数：element p1 p2 p3 p4(arguments like 0.5,0.75,0.435) duration      
在元素内，按比率划动元素<br />
<br />
# get element
参数：locator      
获取指定元素<br />
<br />
<br />
# back to selected view
参数：locator      
从当前页面通过locator回到指定页面，适用于在返回过程中没有弹出确认框的情况，此方法仅对安卓有效<br />
<br />
#以下关键字主要针对get elements获取的列表元素而使用<br />
# get text 
参数：element                 
获取元素的文本属性<br />
# get location          
参数：element                 
获取元素的位置属性<br />
# get size            
参数：element                 
获取元素的大小属性<br />
# select element       
参数：element index        
从webelements元素中根据index，获取指定的webelement元素，用法为 ${el} select element ${els}<br />
# click by element given            
参数：element                 
点击指定元素<br />
# send keys            
参数：element                 
在指定元素内输入<br />

