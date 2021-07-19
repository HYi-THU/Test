# ROS-

ROS安装相关信息

sudo rosdep init ERROR: cannot download default sources list from:【closed】
https://blog.csdn.net/u013468614/article/details/102917569

rosdep init 及update报错的解决办法汇总（亲测）    
https://blog.csdn.net/weixin_39730025/article/details/113348458#commentBox
  
catkin_ws工作空间创建
https://blog.csdn.net/github_30605157/article/details/52209434?


cartograpgher 相关

cartographer使用笔记    
https://blog.csdn.net/weixin_43569276/article/details/112723904?

开源方案安装使用网址
https://google-cartographer-ros.readthedocs.io/en/latest/compilation.html

错误说明
  1. 类似以下代码中路径需改用绝对路径                           
  roslaunch cartographer_ros offline_backpack_2d.launch bag_filenames:=${HOME}/Downloads/b2-2016-04-05-14-44-52.bag
  2. 运行时间较长

配置自己的设备（参考cartograpgher使用笔记）
1. 准备文件   
    在carto_ws/src/cartographer_ros/cartographer_ros/configuration_files中，创建my_mapping_2d.lua    
    在carto_ws/src/cartographer_ros/cartographer_ros/launch中，创建my_mapping_2d.launch
2. 参数设置
    修改my_mapping_2d.lua
