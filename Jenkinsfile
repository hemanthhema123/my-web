pipeline{
    agent any
    stages{
        stage("git"){
            steps{
              git url: 'https://github.com/hemanthhema123/my-web.git'   
            }
        }
        stage("maven"){
            steps{
              sh 'mvn clean package'
            }
        }
    }
}
