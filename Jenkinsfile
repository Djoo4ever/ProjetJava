node {
    stage('Checkout') {
        git branch: 'main', url: 'https://github.com/Djoo4ever/ProjetJava.git'
    }

    stage('Compilation') {
        echo 'Compilation des fichiers Java dans src/...'
        sh 'javac src/HelloWorld.java src/Merci.java src/DeRien.java'
    }

    stage('Execution HelloWorld') {
        echo 'Exécution de HelloWorld.java...'
        sh 'java -cp src HelloWorld'
    }

    stage('Execution Merci') {
        echo 'Exécution de Merci.java...'
        sh 'java -cp src Merci'
    }

    stage('Execution DeRien') {
        echo 'Exécution de DeRien.java...'
        sh 'java -cp src DeRien'
    }

    stage('Fin') {
        echo 'Pipeline terminée avec succès ✅'
    }
}
