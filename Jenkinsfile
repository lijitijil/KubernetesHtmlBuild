pipeline {
    agent any
    stages {
        
        
        stage('git checkout') {
            steps {
                git 'https://github.com/lijitijil/KubernetesHtmlBuild.git'
            }
        }
        stage('git checkout Deploy') {
            steps {
                git 'checkout Deploy'
            }
        }
        stage('deployment') {
            steps{
                sh 'helm install teckask webapp'
            }
        }
    }
}
