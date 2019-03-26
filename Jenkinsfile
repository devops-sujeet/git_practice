@Library('Var-Lib')_

node {
   def mvnHome
   stage('Preparation') { // for display purposes

      git 'https://github.com/devops-sujeet/git_practice.git'
        
     tool name: 'maven3.6', type: 'maven'
   }
   stage('Build') {

      if (isUnix()) {
         sh "'${mvnHome}/bin/mvn' -Dmaven.test.failure.ignore clean package"
      } else {
         bat(/"${mvnHome}\bin\mvn" -Dmaven.test.failure.ignore clean package/)
      }
   }
   stage('Results') {
       echo " Hey! It will work"

   }
   stage('Var-Lib') {
       myclass "sujeet"

   }
}
