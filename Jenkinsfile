pipeline {
  agent any
  stages {
    stage('FETCH CODES FROM SCM[GIT]') {
      steps {
        git(url: 'https://github.com/awsrohit2324/jenkinspract.git', branch: 'main', poll: true)
      }
    }

  }
}