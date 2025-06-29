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
