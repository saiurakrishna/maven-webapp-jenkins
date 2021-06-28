pipeline {
    agent any
    stages { 
        stage('checkout') {
            steps {
            git credentialsId: 'Github-credentials', url: 'https://github.com/saiurakrishna/maven-webapp-jenkins.git'
        }
            
        }
        stage('validate') {
            steps {
                sh 'mvn validate'
            }
        }
        stage('compile') {
            steps {
                sh 'mvn compile'
            }
        }
    }
}
