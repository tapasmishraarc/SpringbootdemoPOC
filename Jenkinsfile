@Library('my-shared-library@main') _

pipeline {
  agent any
 
  tools {maven "MyMaven"}
  parameters {
        string(name: 'url', defaultValue: 'https://github.com/tapasmishraarc/SpringbootdemoPOC.git', description: 'My application url')
    }
  stages {
    stage('CI-Pipeline') {
      steps {
        script {
          
        //readProperties "${params.url}", this
       // echo "${env.APP_NAME}"
         build  "${params.url}", this
        }
        
      }
    }
  }
}

