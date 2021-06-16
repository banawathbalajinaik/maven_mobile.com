pipeline {
    agent any
    stages {
        stage('git_clone') {
            steps {
                sh '''
                rm -rf *
                git clone 'https://github.com/banawathbalajinaik/maven_whatsapp.com.git'
                '''
            }
        }
        stage('mvn_clean') {
            steps {
                sh '''
                pwd
               mvn clean
                '''
            }
        }
        stage('mvn_compile') {
            steps {
                sh '''
                pwd
               mvn compile
                '''
            }
        }
    }
}
