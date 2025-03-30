pipeline {
  agent Node1
  stages {
    stage('FETCH CODES FROM SCM[GIT]') {
      steps {
        git(url: 'https://github.com/awsrohit2324/jenkinspract.git', branch: 'main')
      }
    }

    stage('INSTALL WEB SERVER') {
      steps {
        sh '''sudo apt install apache2 -y
sudo apt install tree -y 
sudo apt install nano -y'''
      }
    }

    stage('DEPLOYMENT OF APPLICATION') {
      steps {
        sh 'sudo cp -R * /var/www/html/'
      }
    }

  }
}
