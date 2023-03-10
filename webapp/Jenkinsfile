pipeline {
    agent any
    stages {
        stage('git checkout') {
            steps {
                git 'https://github.com/lijitijil/KubernetesHtmlBuild.git'
            }
        }
        stage('deployment') {
            steps{
                sh 'helm install teckask webapp'
            }
        }
    }
}
