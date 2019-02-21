pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'php --version'
      }
    }
    stage('deploy') {
      steps {
        openshiftDeploy(depCfg: 'cfg', apiURL: 'hello-world', namespace: 'hello-world')
      }
    }
  }
}
