pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                // Clone la branche main
                git branch: 'main', url: 'https://github.com/Djoo4ever/ProjetJava.git'
            }
        }

        stage('Compilation') {
            steps {
                echo 'Compilation des fichiers Java dans src/...'
                // Compiler tous les fichiers Java dans src/
                sh 'javac src/HelloWorld.java src/Merci.java src/DeRien.java'
            }
        }

        stage('Execution HelloWorld') {
            steps {
                echo 'Exécution de HelloWorld.java...'
                sh 'java -cp src HelloWorld'
            }
        }

        stage('Execution Merci') {
            steps {
                echo 'Exécution de Merci.java...'
                sh 'java -cp src Merci'
            }
        }

        stage('Execution DeRien') {
            steps {
                echo 'Exécution de DeRien.java...'
                sh 'java -cp src DeRien'
            }
        }

    }

    post {
        success {
            echo 'Pipeline terminée avec succès ✅'
        }
        failure {
            echo 'La pipeline a échoué ❌'
        }
    }
}
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

