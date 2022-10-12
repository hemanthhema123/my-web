@Library("hemanth") _
pipeline{
    agent any
    stages{
        stage("git"){
            steps{
              git url: 'https://github.com/hemanthhema123/pipeline.git'   
            }
        }
        stage("maven"){
            steps{
              sh 'mvn clean package'
            }
        }
        stage("tomcat"){
            steps{
             tomcatDeploy("172.31.21.127","ec2-user","tomcat-dev") 
            }
        }
    }
}
