pipeline {
  agent any
  stages {
    stage('Hola Mundo') {
      steps {
        echo 'Hola!'
        sh 'echo %PATH%'
        writeFile(file: 'Prueba.txt', text: 'Prueba Jenkins')
      }
    }

  }
}