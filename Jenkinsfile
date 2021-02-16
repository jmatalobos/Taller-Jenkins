pipeline {
  agent any
  stages {
    stage('Hola Mundo') {
      steps {
        echo 'Hola!'
        bat(script: 'echo %PATH%', returnStdout: true)
      }
    }

    stage('Crear archivo') {
      steps {
        writeFile(file: 'Prueba.txt', text: 'Prueba Jenkins')
      }
    }

  }
}