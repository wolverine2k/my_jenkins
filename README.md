# wolverine2k/my_jenkins
Jenkins image with python &amp; build-essentials

This image is derived from jenkins:1.651.3. It has python-setuptools, python-dev and build-essential installed. So next time you want to install python plugin, you can simply run pip install ... from within your jenkins job itself.

## The image is docker hub. Run docker pull wolverine2k/my_jenkins to get the image

Steps to run the image properly.
1. Create a Container for Jenkins_Home
2. Start this image

eg:
docker create --name jenkins-data-volume -v /data/jenkins_home wolverine2k/my_jenkins /bin/true
docker run -v /data/jenkins_home -d -p 8080:8080 -p 50000:50000 wolverine2k/my_jenkins

ENJOY

Source on #GitHub: https://github.com/wolverine2k/my_jenkins
visit me at: https://www.naresh.se/
