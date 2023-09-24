This project will install jenkins package with all its depencies.

this project will also: 
install And Enable Docker
install Git
Install Java 11:


*** troubleshoot jenkins:
 Try this troubleshouting if the installation doesn't work
 
sudo rm -rf /etc/yum.repos.d/jenkins.repo
sudo yum install -y wget
sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat-stable/jenkins.repo
sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key
sudo yum install -y jenkins
sudo systemctl start jenkins
sudo systemctl enable jenkins
