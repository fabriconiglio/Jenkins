pipeline {
    agent any // Esto especifica que el pipeline puede ejecutarse en cualquier agente disponible en Jenkins.

    stages {
        stage('Bienvenida') { // Primer stage
            steps {
                echo 'Bienvenidos DevOps' // Imprime un mensaje de bienvenida.
            }
        }
        
        stage('Location') { // Segundo stage
            steps {
                script {
                    // Imprime el directorio actual donde se está ejecutando el pipeline.
                    echo "El directorio actual es: ${pwd()}"
                }
            }
        }

        stage('OK') { // Tercer stage
            steps {
                echo 'Build finalizado' // Mensaje de finalización del build.
            }
        }
    }
}
