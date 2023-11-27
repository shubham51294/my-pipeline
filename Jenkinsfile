pipeline {
   agent {
      label {
         label "qa"
         customWorkspace "/mnt/velocity3"
      }
   }
  stages {
     stage ("slave-2") {
        steps {
            sh "sudo git clone https://github.com/shubham51294/my-pipeline.git -b 2023Q2"
            sh "sudo cp -r index.html /var/www/html"
            sh "sudo chmod -R 644 /var/www/html/index.html"
        }
     }
  }
}
