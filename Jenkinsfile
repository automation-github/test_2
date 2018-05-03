pipeline {
  agent any
  environment {
    target_cluster = '10.65.182.142'
  }
  stages {
    stage('test_2') {
      agent any
      steps {
        build (job: 'test_2', propagate: false)
      }
    }

    stage('print_target_cluster') {
      agent any
      steps {
        sh '''echo $target_cluster'''

      }
    }

  }
}
