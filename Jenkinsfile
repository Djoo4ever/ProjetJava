pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Djoo4ever/ProjetJava.git'
            }
        }

        stage('Compilation') {
            steps {
                sh 'javac HelloWorld.java Merci.java DeRien.java'
            }
        }

        stage('Execution') {
            steps {
                sh 'java HelloWorld'
                sh 'java Merci'
                sh 'java DeRien'
            }
        }
    }
}
