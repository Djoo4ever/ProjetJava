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
                echo 'Compilation des fichiers Java...'
                sh 'javac src/HelloWorld.java src/Merci.java src/DeRien.java'
            }
        }

        stage('Execution HelloWorld') {
            steps {
                sh 'java -cp src HelloWorld'
            }
        }

        stage('Execution Merci') {
            steps {
                sh 'java -cp src Merci'
            }
        }

        stage('Execution DeRien') {
            steps {
                sh 'java -cp src DeRien'
            }
        }
    }
}
