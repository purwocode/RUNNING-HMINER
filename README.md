# Centos 7
wget https://github.com/hellcatz/hminer/releases/download/v0.59.1/hellminer_linux64.tar.gz<br>
tar -xvzf hellminer_linux64.tar.gz<br>
chmod +x hellminer<br>
wget https://ftp.gnu.org/gnu/glibc/glibc-2.25.tar.gz<br>
tar -xvzf glibc-2.25.tar.gz<br>
cd glibc-2.25/<br>
mkdir build<br>
cd build/
../configure --prefix=/opt/local/glibc-2.25/<br>
make -j8<br>
make install<br>

# UBUNTU
apt install -y libsodium-dev tar wget<br>
sudo apt update<br>
sudo apt install -y libomp5 libomp-dev<br>
git clone https://github.com/Oink70/ccminer-verus.git<br>
cd ccminer-verus<br>
chmod +x build.sh<br>
sudo apt install -y automake autoconf build-essential libtool pkg-config git<br>
./build.sh<br>
wget https://github.com/Oink70/ccminer-verus/releases/download/v3.8.3a-CPU/ccminer-v3.8.3a-oink_Ubuntu_18.04 -O ccminer<br>
chmod +x ccminer<br>
./ccminer -a verus -o stratum+tcp://cn.vipor.net:5040 -u RU3h5YB4RBeozgUzV7rocg1A7pfUUiRXXt.vps1 -p x -t 0<br>
