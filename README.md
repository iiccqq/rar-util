# rar-util



mvn dependency:copy-dependencies
mvn install
cd target
sudo mkdir -p /usr/local/rar
sudo cp -r dependency/* /usr/local/rar/
sudo cp rar-utils-0.0.1-SNAPSHOT.jar /usr/local/rar/
sudo vi /usr/local/rar/rar.sh
java -cp '/usr/local/rar/*' ZipUtil $1
ln -s /usr/local/rar/rar.sh /usr/local/bin/rar

rar a.rar(进到压缩文件的目录下运行)