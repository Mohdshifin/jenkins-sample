pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                git branch: 'main', url: 'https://github.com/Mohdshifin/jenkins-sample.git'
            }
        }

        stage('Deploy to Apache') {
            steps {
                sh 'sudo cp index.html /var/www/html/index.html'
            }
        }

        stage('Restart Apache') {
            steps {
                sh 'sudo systemctl restart httpd'
            }
        }
    }
}
