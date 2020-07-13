pipeline {
   agent any

   stages {
      stage('Git Checkout') {
         steps {
            // Get some code from a GitHub repository
            git 'https://github.com/fahimrahmanbooom/Portfolio.git'

         }
      }
      stage('Deploy') {
         steps {
            sh """
            rm -rf /var/www/html/fahim
            mkdir /var/www/html/fahim
            mv * .[^.]* /var/www/html/fahim/
            """

         }
      }

   }
}
