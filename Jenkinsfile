pipeline {
    agent any

    stages {
        stage('Creation') {
            steps {
                script {
                    // Crear una carpeta y un archivo dentro de ella
                    sh '''
                    mkdir -p nueva_carpeta
                    echo "Contenido del archivo" > nueva_carpeta/archivo.txt
                    '''
                }
            }
        }

        stage('Copy') {
            steps {
                script {
                    // Copiar el archivo en la carpeta /tmp/files
                    sh '''
                    mkdir -p /tmp/files
                    cp nueva_carpeta/archivo.txt /tmp/files/archivo.txt
                    '''
                }
            }
        }

        stage('Delete') {
            steps {
                script {
                    // Eliminar el archivo original
                    sh '''
                    rm -rf nueva_carpeta
                    '''
                }
            }
        }
    }
}
