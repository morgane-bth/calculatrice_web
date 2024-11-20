pipeline {
  agent any
  stages {
    stage('Build'){
      steps {
        echo 'Building'
        bat 'node app.js'
      }
    }
    stage ('Check for existence of index.html') {
    steps {
        script {
            if (fileExists('index.html')) {
                echo "File index.html found!"
            }
        }
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