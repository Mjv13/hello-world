pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        build 'build'
      }
    }
    stage('deploy') {
      steps {
        openshiftDeploy(depCfg: 'cfg', apiURL: 'hello-world', namespace: 'hello-world')
      }
    }
  }
}