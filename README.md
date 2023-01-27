# Jenkins_Documentaion
CI server Jenkins Documentation
Follow the below link to install the jeknkins
https://devopscube.com/install-configure-jenkins-2-centos-redhat-servers/

To Install specific version follow the link: https://get.jenkins.io/redhat/

java default path : /usr/lib/jvm/java-11-openjdk-11.0.16.0.8-1.amzn2.0.1.x86_64/bin

    1  
    2  sudo yum install wget git -y
    3  sudo amazon-linux-extras install java-openjdk11
    4  java -version
    5  
    6  ll /usr/lib/jvm/java-11-openjdk-11.0.16.0.8-1.amzn2.0.1.x86_64
    7  vi ~/.bashrc
    8  source ~/.bashrc
    9  echo $JAVA_HOME
   10  sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat/jenkins.repo
   11  sudo rpm --import https://pkg.jenkins.io/redhat/jenkins.io.key
   12  sudo yum install jenkins
   13  sudo systemctl daemon-reload
   14  sudo systemctl enable jenkins
   15  sudo systemctl status jenkins
   16  sudo systemctl start jenkins
   17  sudo systemctl status jenkins
   18  sudo cat /var/lib/jenkins/secrets/initialAdminPassword
   19  sudo vi /etc/sudoers
   20  jenkins ALL=(ALL)       NOPASSWD: ALL

  
  
