pipeline {
   agent {
      label {
         label "built-in"
         customWorkspace "/mnt/velocity"
      }
   }
  stages {
     stage ("on-master") {
        steps {
            sh "cp -r index.html /var/www/html"
            sh "chmod -R 644 /var/www/html/index.html"
        }
     }
  }
}
