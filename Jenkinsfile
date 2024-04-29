pipeline {
    agent any

    parameters {
        string(name: 'USER_NAME', defaultValue: 'JUAN PEREZ', description: 'Ingrese su nombre completo')
        choice(name: 'AWS_PROFILE', choices: ['inkcluster-dev', 'inkcluster-prod', 'inkcluster-test'], description: 'Seleccione la cuenta AWS')
        choice(name: 'AWS_REGION', choices: ['us-east-1', 'us-east-2', 'us-west-1'], description: 'Seleccione la región AWS')
    }

    stages {
        stage('Set Environment') {
            steps {
                script {
                    // Imprimir un mensaje de bienvenida con las variables seleccionadas
                    echo "Bienvenido ${params.USER_NAME}, estás en la cuenta ${params.AWS_PROFILE} en la región ${params.AWS_REGION}."
                }
            }
        }
    }
}
