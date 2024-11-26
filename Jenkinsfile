pipeline {
    agent {
        docker {
            image 'jenkins/inbound-agent:latest'
        }
    }
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Run Script') {
            steps {
                sh './script.sh'
            }
        }
    }
}
