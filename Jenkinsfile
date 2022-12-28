pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        echo 'Hello World'
        git(url: 'https://github.com/mdrajibkhan/webservercicd.git', branch: 'main', poll: true)
      }
    }

    stage('test-stage') {
      steps {
        sh 'echo "Testing"'
      }
    }

    stage('Deployment') {
      steps {
        echo 'Deploying Application'
      }
    }

  }
}