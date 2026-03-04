pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/BUdayKumarReddy/taskcli-static-website.git'
            }
        }

        stage('Verify Files') {
            steps {
                sh 'ls -la'
            }
        }

        stage('Build') {
            steps {
                echo "Static website - No build required"
            }
        }
    }
}
