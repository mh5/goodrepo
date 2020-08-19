pipeline {
  agent any
  parameters {
    string(name: 'Greeting', defaultValue: 'Hello', description: 'How should Igreet the world?')
  }
  
  stages {
    stage('Build') {
      steps {
        echo "lol ${params.Greeting}"
        sh false
      }
    }
  }
  
  post {
    failure {
      echo "things went bad, buddy."
    }
  }
}
