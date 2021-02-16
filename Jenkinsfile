pipeline {
  agent any
  stages {
    stage('Hola Mundo') {
      steps {
        echo 'Hola!'
        bat(script: 'set', returnStdout: true, returnStatus: true)
        bat(script: 'set Nombre=Juanma', returnStdout: true, returnStatus: true)
        bat(script: 'echo %Nombre%', returnStatus: true, returnStdout: true)
      }
    }

    stage('Crear archivo') {
      steps {
        writeFile(file: 'Prueba.txt', text: 'Prueba Jenkins')
      }
    }

    stage('Despedida') {
      steps {
        input(message: 'Lástima que terminó', ok: 'Excelente taller!')
      }
    }

  }
}