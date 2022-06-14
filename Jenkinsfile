pipeline {
  agent {
    label 'maven'
  }
  parameters {
    booleanParam(name: 'CLEAN_BEFORE_BUILD', description: 'Limpar o workspace antes de rodar o build')
  }
  stages {
    state('Clean') {
      when {
        expression { params.DEBUG_BUILD }
      }
      steps {
        echo 'Stage clean!'
      }
    }
    stage('Compile') {
      steps {
        echo 'Stage compile!'
      }
    }
    stage('Test') {
      steps {
        echo 'Stage test!'
      }
    }
  }
}