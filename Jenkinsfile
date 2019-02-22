pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo "Build completed!"
      }
    }
    stage('deploy') {
      steps {
        openshiftDeploy(depCfg: 'cfg', apiURL: 'hello-world', namespace: 'hello-world')
      }
    }
  }
}
