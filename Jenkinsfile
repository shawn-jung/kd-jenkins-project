pipeline {
    agent {
        docker {
            image 'python:3.11'
            }
        }
    stages {

        stage('Checkout') {
            steps {
                git url: 'https://github.com/shawn-jung/kd-jenkins-project.git', branch: 'main'
                sh "ls -ltr"
                echo "super ikkulim"
            }

        }
        stage('Setup') {
            steps {
                sh "pip install -r requirements.txt"
            }
        }
        stage('Test') {
            steps {
                sh "pytest"
                sh "whoami"
            }
        }

    }
}