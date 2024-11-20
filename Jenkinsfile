pipeline {
  agent any
  stages {
    stage('Build'){
      steps {
        echo 'Building'
        bat 'node app.js'
      }
    }
    stage('Test'){
      steps {
        def exists = fileExists 'index.html'
        if (exists) {echo 'index.html existe'}
        else {echo 'index.html n existe pas'}
    }
  }
}
}