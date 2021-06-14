pipeline {
    agent any
    tools {
        jdk 'JDK11'
    }
    stages {
        stage('build') {
            steps {
                echo 'Build started'
                bat 'mvn --version'
                bat 'mvn clean compile'
                echo 'Build Compiled Succesfully'
                bat 'mvn test'
                echo 'Build Finished Succesfully'
            }
        }
    }
}