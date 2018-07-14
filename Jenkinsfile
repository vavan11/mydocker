pipeline {
  agent any
  stages {
    stage('Install net-tool') {
      steps {
        sh '''HOSTIP=$(cat /bitnami/gateway)
ssh -i /bitnami/ssh/id_rsa -oStrictHostKeyChecking=no metaxa@${HOSTIP} pwd'''
      }
    }
  }
}