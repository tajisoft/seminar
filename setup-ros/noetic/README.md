# ROSセットアップ
## Ubuntu 20向け
ターミナルアプリを起動して次のコマンドを順番に実行して必要なソフトウェアをインストールします。コマンド実行結果が正常な場合のみ続けてください。エラーが発生している場合は継続して実行してもセットアップが完了しません。
```
$ sudo apt update

$ sudo apt upgrade -y

$ sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

$ sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

$ sudo apt update

$ sudo apt install ros-noetic-desktop-full

$ echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
source ~/.bashrc

$ sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential

$ sudo apt install python3-prettytable

$ sudo apt install python3-rosdep

$ sudo rosdep init

$ rosdep update
```

PCを再起動してください。
