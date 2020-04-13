pipeline {
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
                sh 'mvn clean'
                sh 'mvn package'
                sh 'pwd'
                sh 'ls'
                sh 'ls target'
                sh 'ls target/classes'
                sh 'java -cp target.classes helloworld.HelloWorld'
            }
        }
    }
}