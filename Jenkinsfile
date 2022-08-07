pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'build stage'
          }
        }

        stage('parallel build') {
          steps {
            echo 'parallel build'
          }
        }

      }
    }

    stage('test') {
      steps {
        echo 'test'
      }
    }
    
    stage('ci') {
      steps {
        echo 'ci pipeline'
      }
    }

    stage('delever') {
      steps {
        echo 'delever'
      }
    }

  }
  environment {
    prod = ''
  }
}
