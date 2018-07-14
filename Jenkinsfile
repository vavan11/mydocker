pipeline {
  agent any
  stages {
    stage('ssh') {
      steps {
        sh '''#!/bin/bash -v
HOSTIP=$(cat /bitnami/gateway)
ssh -i /bitnami/ssh/id_rsa -oStrictHostKeyChecking=no metaxa@${HOSTIP} ls'''
      }
    }
  }
}