pipeline {
  agent any
  stages {
    stage('stage 1') {
      parallel {
        stage('stage11') {
          steps {
            sh 'cut  -d : -f1,3 /etc/passwd > /tmp/users'
          }
        }

        stage('stage12') {
          steps {
            sh 'cut -d: -f1,3 /etc/group > /tmp/groupes'
          }
        }

      }
    }

    stage('stage 2') {
      steps {
        sh 'cut -d: -f4 /etc/passwd | sort|uniq > /tmp/group_prim'
      }
    }

  }
}