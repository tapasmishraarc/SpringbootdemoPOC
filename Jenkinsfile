@Library('my-shared-library@master') _

pipeline {
  agent any
 
  tools {nodejs "nodejs"}
  parameters {
        string(name: 'url', defaultValue: 'https://github.com/tapasmishraarc/sample-nodejs.git', description: 'My application url')
    }
  stages {
    stage('CI-Pipeline') {
      steps {
        script {
          
        //readProperties "${params.url}", this
        echo "${env.APP_NAME}"
         build  "${params.url}", this
        }
        
      }
    }
  }
}

