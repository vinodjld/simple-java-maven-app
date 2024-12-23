pipeline {
    agent any
    tools {
        maven 'MAVEN_3.9.9' 
    }
    stages {
        stage('SCM') {
            steps {
                git url : 'https://github.com/vinodjld/simple-java-maven-app.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn build'
            }
        }
    }
}
