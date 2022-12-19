pipeline {
    agent any 
    stages {
        stage('Git Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Teja-Aws/Sample.git'
                  }
                              }
        
        stage('Deploy') { 
            steps {
                sh 'cp -R * /var/www/html/'
                  }
                         }
        
            }
}
