#!/usr/bin/env groovy
pipeline{
  agent none
  stages{
    stage("Hii"){
      agent{
        node{
          label 'ngbuilda02'
        }
      }
      steps{
        checkout scm
        echo "Hiis"
        echo "Current workspace is ${env.WORKSPACE}"
      }
    }
  }
}
