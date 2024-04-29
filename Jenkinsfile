pipeline {
    agent any  // Este pipeline puede ejecutarse en cualquier agente disponible

    stages {
        stage('Set AWS Environment Variables') {
            steps {
                script {
                    // Establecer las variables de entorno
                    env.AWS_PROFILE = 'inkcluster-dev'
                    env.AWS_REGION = 'us-east-2'

                    // Imprimir las variables de entorno para validar
                    echo "AWS_PROFILE is set to: ${env.AWS_PROFILE}"
                    echo "AWS_REGION is set to: ${env.AWS_REGION}"
                }
            }
        }
    }
}
