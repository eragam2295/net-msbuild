pipeline {
    agent any
    tools {
        jdk 'java'
        git 'Default'
        msbuild 'msbuild'
    }
    stages {
        stage('---msbuild---') {
            steps {
                sh "msbuild HelloWorld.sln"
            }
        }
        
        stage('---mstest---') {
            steps {
                sh "msbuild HelloWorld.csproj /t:RunUnitTests"           
                 
         }
        }
    }
                
   
    }
