pipeline {
   agent {
      label {
         label "dev"
         customWorkspace "/mnt/velocity2"
      }
   }
  stages {
     stage ("slave-1") {
        steps {
            sh "rm -rf *"
            sh "yum install git -y"
            sh "yum install httpd -y"
            sh "systemctl start httpd"
            sh "cp -r index.html /var/www/html"
            sh "chmod -R 644 /var/www/html/index.html"
        }
     }
  }
}
