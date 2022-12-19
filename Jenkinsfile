pipeline {
    agent any 
    stages {
        stage('Git Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Teja-Aws/Sample.git'
                  }
                              }
        stage('Changing User/Group and Permission') {
            steps {
                sh 'whoami'
                sh 'chmod -R 777 /var/lib/jenkins/workspace/sample-pipe'
                sh 'chown -R jenkins:jenkins /var/www/html/'
                  }
        
                             } 
        stage('Deploy') { 
            steps {
                sh 'sudo cp -R * /var/www/html/'
                  }
                         }
        
            }
}
