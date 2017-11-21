# OYA-1003
Automated Guided Vehicle simulation
Dosyaları catkin_ws/src dosyasının altına yerleştiriniz. "workcell" ve "workcell_bin" dosyaları model dosyalarıdır. Bu modellerin dünyaya kolay eklenebilmesi için bashrc belgesine 
#### $ export GAZEBO_MODEL_PATH=/home/[kullanıcı adınız]/catkin_ws/src 
komutunu yazınız.
Dünyayı çalıştırmak için terminale
#### $ catkin_make
#### $ source catkin_ws/devel/setup.bash
#### $ roslaunch agvcasterwheel_gazebo agvcasterwheel.launch 
komutu ile simülasyon ortamı çalıştırılabilir.

Ariac ortamı kullanılan bu simülasyonda isimleri: agv1, agv2 ve agv3 olmak üzere 3 tane OYA bulunmaktadır. 
Her bir topik robotun ismi ile başlar. 

Robotun başlangıç yerleri değiştirilmek istenirse agvcasterwheel.launch belgesinde "x","y", 
baş açısı değiştirilmek istenirse "yaw" parametleri değiştirilmelidir.

##### Robotların /cmd_vel topikleri farklı terminallerden yayınlanmalıdır.
