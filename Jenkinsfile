
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Jenkins is connected to the Laravel project!'
                sh 'git --version'
                sh 'php --version'
            }
        }

        stage('Verify Laravel') {
            steps {
                sh 'test -f artisan'
                sh 'test -f composer.json'
                sh 'echo "Laravel project files verified"'
            }
        }
    }
}
