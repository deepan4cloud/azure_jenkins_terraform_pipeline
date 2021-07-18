pipeline{
       agent any
stages{
    stage('Checkout') {
      steps {
            git branch: 'master',
                credentialsId: 'deepan4cloud-git-cred',
                url: 'https://github.com/deepan4cloud/azure_jenkins_terraform_pipeline.git'

            sh "pwd"
            sh "ls -lat"
        }
    }

    stage('Set Terraform path') {
    steps {
      script {
        def tfHome = tool name: 'terraform'
        env.PATH = "${tfHome}:${env.PATH}"
       }
       sh 'terraform version'

      }
    }
