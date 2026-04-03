pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Compilando el proyecto...'
                echo 'Compilando el proyecto... v2'
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
