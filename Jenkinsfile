pipeline {
    agent any
    stages {
        stage('Info') {
            steps {
                echo "Nombre del Job: ${env.JOB_NAME}"
                echo "Numero de Build: ${env.BUILD_NUMBER}"
                echo "URL del Build: ${env.BUILD_URL}"
                echo "Rama: ${env.GIT_BRANCH}"
            }
        }        
        stage('Build') {
            steps {
                echo 'Compilando el proyecto...'
                echo 'Compilando el proyecto... v2'
                echo 'Compilando el proyecto... v3.1'
                echo 'Build exitoso!'
            }
        }
        stage('Test') {
            steps {
                echo 'Ejecutando pruebas...'
                echo 'Todas las pruebas pasaron!'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Desplegando la aplicacion...'
                echo 'Deploy exitoso!'
            }
        }
    }
    post {
        success {
            echo 'Pipeline completado exitosamente!'
        }
        failure {
            echo 'Algo salio mal!'
        }
    }
}
