pipeline {
    agent any
stages {
    stage('Build') {
            steps {
                echo 'Compilation du projet...'
                echo 'Packaging en cours...'
            }
        }

     stage('Tests') {
            steps {
                echo 'Lancement des tests unitaires...'
                echo 'Lancement des tests d’intégration...'
                echo 'Génération du rapport de tests...'
                script {
                    if (fileExists('index.html')) {
                        echo "✅ Fichier index.html trouvé !"
                    } else {
                        error "❌ Fichier index.html manquant !"
                    }
                }
            }
        }
}
}