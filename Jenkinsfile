pipeline {
  agent any
  parameters {
    gitParameter branchFilter: 'origin/(.*)', defaultValue: 'master', name: 'VERSION', type: 'PT_VERSION'
  }
  stages {
    stage('Example') {
      steps {
        git version: "${params.VERSION}", url: 'https://github.com/witsutaOn/jenkins-test.git'
      }
    }
  }
}