**ROS配置过程**

step1：Setup your sources.lis</br>代码：<em>sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'</em></br>
&nbsp;我们设置计算机的source，以接受来自packages.ros.org软件</br>
step2: Set our keys</br>代码：<em>sudo apt-key adv --keyserver hkp://ha.pool.sks-keyservers.net:80 --recv-key 0xB01FA116</em>
>![hello world](https://github.com/laiCheung/Picture/blob/master/1.jpg?raw=true)

step3:Install ROS配置过程
</br>&emsp;首先，我们需要把我们的系统的package更新到最新
</br>&emsp;&emsp;<em>sudo apte-get update</em>
</br>&emsp;然后暗转ROS，因为ROS有不同库和工具，开发者提供了四种不同版本，我们选择Desktop-Install full版本，因为这个版本提供了最为全面的工具，包括2D,3D等
> ![hello world](https://github.com/laiCheung/Picture/blob/master/2-ros.jpg?raw=true)

step4:初始化rosdep
</br>&emsp;为可以使用ROS，您将需要初始化rosdep。rosdep使您可以轻松地安装系统的依赖关系为要编译和运行要求的ROS一些核心部件来源。
</br><em>&emsp;sudo rosdep init
</br>&emsp;rosdep update</em>
> ![hello world](https://github.com/laiCheung/Picture/blob/master/3-init.jpg?raw=true)</br>

> ![hello world](https://github.com/laiCheung/Picture/blob/master/4.jpg?raw=true)

step4:环境配置
如果ROS环境变量的每一个新的shell启动时自动添加到您的bash命令：
<br>&emsp;<em>echo "source /opt/ros/kinetic/setup.bash" >> ~/.bashrc
<br>&emsp;source ~/.bashrc</em>
</br>因为我们并不是安装了分布式的ROS

>![hello world](https://github.com/laiCheung/Picture/blob/master/5.jpg?raw=true)

step6:获取rosinstall
</br>rosinstall是ROS经常使用的命令行工具，单独发行。它使您能够轻松下载许多源代码树的ROS包使用一个命令。
</br><em>&emsp;sudo apt-get install python-rosinstall</em>

>![hello world](https://github.com/laiCheung/Picture/blob/master/6-down.jpg?raw=true)

step7:测试一下我们安装的结果罗







