pipeline{
 agent{label 'slave'}

stages{
stage('scm'){
steps{
checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'bb5d31f0-16de-4816-baa8-a717af9be3d8', url: 'https://github.com/flyhighhhh/mavenrepo.git']]])
 
      }

       }

stage{
steps{
sh 'mv package'
      }
      }
}
         }
