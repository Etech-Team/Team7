#!/bin/bash 
#This is a Jenkins script to Etech Devops
Pipeline{
    agent any
    Stages{
        stage('1-JenkinsStatus'){ 
            steps{
                sh 'sudo systemctl status jenkins'
            }
        }
        stage('parallel'){
        parallel{
            stage('2-1 DiskCheck1'){
                steps{
                    sh 'df -h'
                }
            }
            stage('2-2 DiskCheck2'){
                steps{
                    sh 'du -h'
                    }
               }
             }       

        }
 
    }
}
