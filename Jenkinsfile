pipeline {
    agent any  // Asegura que el Job puede ejecutarse en cualquier agente disponible

    stages {
        stage('Check Docker Version') {
            steps {
                script {
                    // Ejecutar el comando para obtener la versión de Docker
                    def dockerVersion = sh(script: 'docker --version', returnStdout: true).trim()
                    echo "La versión de Docker instalada es: ${dockerVersion}"
                }
            }
        }
    }
}
