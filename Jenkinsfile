pipeline {
  agent any
  stages {
    stage('Install net-tool') {
      steps {
        sh '''#!/bin/bash -x -v
apt update && apt install -y net-tools


'''
      }
    }
  }
}