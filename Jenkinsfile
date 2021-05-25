pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo build'
      }
    }

    stage('backend') {
      parallel {
        stage('unit') {
          steps {
            sh 'echo unit'
          }
        }

        stage('performance') {
          steps {
            sh 'echo step'
          }
        }

      }
    }

    stage('Frontend') {
      steps {
        sh 'echo Fromtend'
      }
    }

    stage('static') {
      steps {
        sh 'echo Static'
      }
    }

    stage('Deploy') {
      steps {
        sh 'echo Deploy'
      }
    }

  }
}