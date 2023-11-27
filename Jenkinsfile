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
            sh "sudo git clone https://github.com/shubham51294/my-pipeline.git -b 2023Q1"
            sh "sudo cp -r index.html /var/www/html"
            sh "sudo chmod -R 644 /var/www/html/index.html"
        }
     }
  }
}
