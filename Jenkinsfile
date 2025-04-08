pipeline {
    agent any
    stages {

        stage('Checkout') {
            steps {
                git url: 'https://github.com/shawn-jung/kd-jenkins-project.git', branch: 'main'
                sh "ls -ltr"
                echo "super ikkulim"
            }
        }
        stage('Test') {
            steps {
                sh "whoami"
            }
        }

    }
}