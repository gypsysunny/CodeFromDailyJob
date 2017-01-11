# CodeFromDailyJob
记录一下ubuntu16.04安装Nvidia cudn cudaa的过程
1）ubuntu的安装使用U盘，细节百度
2）cuda、cudnn安装，参考：http://askubuntu.com/questions/451221/how-do-i-install-the-nvidia-driver-for-a-geforce-gt-630
add the graphics-drivers ppa
sudo add-apt-repository ppa:graphics-drivers/ppa
sudo apt-get update
install the recommended driver
sudo ubuntu-drivers autoinstall
restart your system
sudo reboot
To select a different driver, or if the above doesn't work:

add the graphics-drivers ppa
sudo add-apt-repository ppa:graphics-drivers/ppa
sudo apt-get update
purge any existing nvidia related packages you have installed
sudo apt-get purge nvidia*
check which drivers are available for your system
ubuntu-drivers devices
install the recommended driver
sudo apt-get install nvidia-361
restart your system
sudo reboot
（不需要参考其它方法，容易造成安装后进入不了图形界面）
其余百度
