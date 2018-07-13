pipeline {
  agent any
  stages {
    stage('ssh') {
      steps {
        sh '''#!/bin/bash
set -x
XYZ=$(expect -c "
spawn ssh-keygen -b 2048 -t rsa -q
expect \\"Enter passphrase (empty for no passphrase):\\"
send \\"\\r\\"
expect \\"Enter same passphrase again:\\"
send \\"\\r\\"
")'''
      }
    }
  }
}