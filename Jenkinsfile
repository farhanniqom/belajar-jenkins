pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'git@github.com:farhanniqom/belajar-jenkins.git'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                sudo rm -rf /var/www/html/*
                sudo cp -r * /var/www/html/
                '''
            }
        }
    }
}