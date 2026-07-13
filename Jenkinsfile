pipeline {
    agent any 

    stages {
        stage('Clonar Codigo') {
            steps {
                checkout scm
            }
        }
        
        stage('Compilar con GCC') {
            steps {
                sh 'gcc -o mi_programa main.c'
            }
        }
        
        stage('Probar Ejecucion') {
            steps {
                sh './mi_programa'
            }
        }
    }
}
