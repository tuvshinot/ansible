# Install
cd ~/
wget -O ~/gradle-4.7-bin.zip https://services.gradle.org/distributions/gradle-4.7-bin.zip
sudo yum -y install unzip java-1.8.0-openjdk
sudo mkdir /opt/gradle
sudo unzip -d /opt/gradle/ ~/gradle-4.7-bin.zip

# Adding gradle PATH
sudo vi /etc/profile.d/gradle.sh
export PATH=$PATH:/opt/gradle/gradle-4.7/bin
sudo chmod 755 /etc/profile.d/gradle.sh

#Logout and back then ->  Check
gradle --version


