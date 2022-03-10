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
                bat 'mvn verify sonar:sonar -Dlogin=admin -Dpassword=admin2'
            }
        }
    }
}