pipeline {
    agent any  // El job puede ejecutarse en cualquier agente disponible

    stages {
        stage('Display Directory') {
            steps {
                script {
                    // Comando para imprimir el directorio actual
                    def currentDir = sh(script: 'pwd', returnStdout: true).trim()
                    echo "El directorio actual es: ${currentDir}"

                    // Imprimir la marca de agua
                    echo "MIGRA Ink. All rights reserved ©"
                }
            }
        }
    }
}
