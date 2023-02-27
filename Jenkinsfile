pipeline {
  agent any
  stages {
  
stage('helm repo check out ') {
      steps {
      git branch: 'main', url: 'https://github.com/vinopandi/terraform.git'
      }
    }
stage('deploy to helm ') {
      steps {
            sh 'terraform init'
            sh 'terraform apply'
            }
    }
}
}
