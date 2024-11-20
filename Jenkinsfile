pipeline {
  agent any
  stages {
    stage('Build'){
      steps {
        echo 'Building'
        bat 'node app.js'
      }
    }
    // stage('Test'){
    //   steps {
    //     set exists = fileExists 'index.html'
    //     If (exists) {echo 'index.html existe'}
    //     ELSE {echo 'index.html n existe pas'}
    //   }
    // }
  }
}