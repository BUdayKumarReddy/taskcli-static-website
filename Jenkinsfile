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
                sudo rm -rf /usr/share/nginx/html/*
                sudo cp -r * /usr/share/nginx/html/
                sudo systemctl restart nginx
                '''
            }
        }
    }
}
