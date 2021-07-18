pipeline{
       agent any

stage ('checkout') {
        checkout([$class: 'GitSCM', branches: [[name: '*/main']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '', url: 'https://github.com/deepan4cloud/azure_jenkins_terraform_pipeline.git']]])      
        }
}
