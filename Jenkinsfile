pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git url: 'https://github.com/Djoo4ever/ProjetJava.git', branch: 'main'
            }
        }

        stage('Compilation') {
            steps {
                sh '''
                    echo "Compilation des fichiers Java..."
                    javac HelloWorld.java Merci.java DeRien.java
                '''
            }
        }

        stage('Execution HelloWorld') {
            steps {
                sh '''
                    echo "--- Execution HelloWorld.java ---"
                    java HelloWorld
                '''
            }
        }

        stage('Execution Merci') {
            steps {
                sh '''
                    echo "--- Execution Merci.java ---"
                    java Merci
                '''
            }
        }

        stage('Execution DeRien') {
            steps {
                sh '''
                    echo "--- Execution DeRien.java ---"
                    java DeRien
                '''
            }
        }

    }
}
