pipeline {
    agent any

    stages {

        stage('Verify Files') {
            steps {
                sh 'ls -la'
            }
        }

        stage('Deploy to Nginx') {
            steps {
                sh '''
                rm -rf /usr/share/nginx/html/*
                cp -r * /usr/share/nginx/html/
                '''
            }
        }
    }
}
