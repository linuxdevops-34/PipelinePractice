pipeline{
    agent any
       tools {
          maven 'maven'
             }
    stages{
        stage("Git Checkout"){
            steps{
                git credentialsId: 'github', url: 'https://github.com/devopsarchitecture/SampleMavenBuild.git'
            }
        }
        stage("Build"){
            steps{
                sh "clean mvn package"
            }
        }
    }
  
}
      
