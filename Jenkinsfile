pipeline {
  agent any
  stages {
    stage('export_LCR') {
      parallel {
        stage('export_LCR') {
          steps {
            sh 'export.sh etc.'
          }
        }
        stage('export common projects') {
          steps {
            sh 'export.sh ....'
          }
        }
      }
    }
    stage('transformation') {
      steps {
        sh 'cp..'
      }
    }
    stage('code inspection') {
      steps {
        isUnix()
      }
    }
  }
}