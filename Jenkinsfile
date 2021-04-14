library identifier: 'Vanshika-Libraries@master',
    //'master' refers to a valid git-ref
    //'mylibraryname' can be any name you like
    retriever: modernSCM([
      $class: 'GitSCMSource',
      //credentialsId: 'your-credentials-id',
      remote: 'https://github.com/Vanshika4222/jenkins-shared-library.git'
])

  pipeline {
       agent any
       tools {
           maven "MyMaven"
           jdk "MyJDK"
       }
       stages {
           stage('Demo') {
                steps {
                    echo 'Hello Vanshika'
                    mavenBuild 'https://github.com/Vanshika4222/SpringbootdemoPOC.git'
                    //notify "type:'slack' message:'a slack notification'"
                }
            }
        }
    }
