# SUSTC_ROS

@gcy, 你在robot.urdf更新一下雷达部分的代码，或者如果你如果写了别的文件你上传更新一下。

@关于地图
这次新传的robot压缩包里面包括了地图和其他已经更改过的部分，如果你想省劲就直接下载

如果你不想重新下一次:
地图文件是那个roommap.world:
   你需要在robot 下创建一个worlds文件夹，然后把roommap.world放进去
   另外需要在launch里面增加world.launch文件
 
 运行方法：  运行的时候直接运行那个world.launch文件就可以在gezobo里面看到完整的包括地图和robot的模型
 
@ about kinect to build SLAM map
i have upload the file of world.launch. plase raw the code and dowanload depthimag-to-laserscan package.

when you want to roslaunch it, you just launch world.lauch and then 
$ rosrun depthimage_to_laserscan depthimage_to_laserscan image:=/kinect1/depth/image_raw
