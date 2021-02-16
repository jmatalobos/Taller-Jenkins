pipeline {
  agent any
  stages {
    stage('Hola Mundo') {
      steps {
        echo 'Hola!'
        bat(script: 'set', returnStdout: true, returnStatus: true, label: 'set')
        bat(script: 'set Nombre=Juanma', returnStdout: true, returnStatus: true, label: 'set2')
        bat(script: 'echo %Nombre%', returnStatus: true, returnStdout: true, label: 'echo')
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