pipeline {
    agent any 
    stages {
        stage('Git Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Teja-Aws/Sample.git'
                  }
                              }
        stage('Email notification') {
            steps {
          emailext body: 'successfully triggred', subject: 'job', to: 'tejathotadevops2@gmail.com'
                  }
        
                             } 
        stage('Deploy') { 
            steps {
                sh 'sudo cp -R * /var/www/html/'
                  }
                         }
        
            }
}
