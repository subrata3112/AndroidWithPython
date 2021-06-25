I tried building APKs using python for small desktop applications.
I used two modules of python
  1. Kivy
  2. Buildozer

How to set-up Kivy and Buildozer:
  1. pip3 install kivy
  2. pip3 install buildozer
  3. Installing dependencies for buildozer
      sudo apt install -y git zip unzip openjdk-8-jdk python3-pip autoconf libtool pkg-config zlib1g-dev libncurses5-dev libncursesw5-dev libtinfo5 cmake libffi-dev libssl-dev
pip3 install --user --upgrade Cython==0.29.19 virtualenv  # the --user should be removed if you do this in a venv

How to make an APK out of Kivy program:
  1. Name your python(Kivy) file as main.py
  2. In the same directory open a terminal and run -> buildozer -v android debug
  3. After the process is complete, you will find the apk in bin folder.
