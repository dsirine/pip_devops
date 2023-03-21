pipeline {
  agent any
  stages {
    stage('') {
      steps {
        sh 'sh \'cut -d: -f1,3 /etc/passwd > /tmp/users\''
        sh 'sh \'cut -d: -f1,3 /etc/group > /tmp/groupes\''
      }
    }

  }
}