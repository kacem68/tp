pipeline {
    agent any
    tools {
        maven 'Maven '
        jdk 'jdk1.8.0_201'
    }
    stages {
        stage ('Build') {
            steps {
                bat 'mvn install'
            }
            post {
                success {
                    junit 'target/surefire-reports/**/*.xml'
                }
            }
        }
    }
}
