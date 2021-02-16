pipeline {
  agent any
  stages {
    stage('Hola Mundo') {
      steps {
        echo 'Hola!'
        bat(script: 'set', returnStdout: true)
        sh '''SET Nombre=Juanma
ECHO %Nombre%'''
      }
    }

    stage('Crear archivo') {
      steps {
        writeFile(file: 'Prueba.txt', text: 'Prueba Jenkins')
      }
    }

  }
}