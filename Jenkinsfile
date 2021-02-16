pipeline {
  agent any
  stages {
    stage('Hola Mundo') {
      environment {
        Prueba = 'Juanma'
      }
      steps {
        echo 'Hola!'
        bat(script: 'set', returnStdout: true, returnStatus: true, label: 'set')
        bat(script: 'echo %PATH%', label: 'echo', returnStatus: true, returnStdout: true)
        bat(script: 'set Nombre=Juanma', returnStdout: true, returnStatus: true, label: 'set2')
        bat(script: 'echo %Nombre%', returnStatus: true, returnStdout: true, label: 'echo')
        bat(script: 'echo %Prueba%', label: 'prueba', returnStatus: true, returnStdout: true)
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