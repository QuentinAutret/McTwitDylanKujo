pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                bat 'mvn install'
            }
        }
        stage('sonar') {
            steps {
                bat 'mvn verify sonar:sonar -Dsonar.login=admin -Dsonar.password=admin2'
            }
        }
    }
}