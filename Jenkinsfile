pipeline {
  agent {label:'worker_node' }
  stages {
    stage('test') {
      sh 'ip addr'
      git 'git@github.com:Dimple-Wmj/python_test.git'
    }
  }
}
