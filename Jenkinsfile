#!/usr/bin/env groovy
pipeline{
  agent none
  stages{
    stage("Hii"){
      agent any
      steps{
        checkout scm
        echo "Hiis"
        echo "Current workspace is ${env.WORKSPACE}"
         sshagent(credentials : ['hraj']) {
                    sh 'ssh -oStrictHostKeyChecking=no fxdeva11 echo "test connect -v $(echo "${VERSION}")"'
         }
      }
    }
  }
}
