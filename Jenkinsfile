pipeline {
  agent {label "built-in"}
  stages {
    stage('Hello') {
      steps {
        echo "Hello from Jenkinsfile"
      }
    }
    stage('For the test branch') {
      when {
        branch "*test*"
      }
      steps {
        echo "If you see this, then it is from test branch :P"
      }
    }
    stage('For the PR branch') {
      when {
        branch "PR-*"
      }
      steps {
        echo "If you see this, then it is from PR branch. You may do pull request and accept it"
      }
    }
  }
}
