pipeline{
    agent any
    
    enviornment{
        PATH="C:\Program Files\Maven\apache-maven-3.6.3-bin\apache-maven-3.6.3\bin:$PATH"
    }
    stages{
        stage("Git checkout"){
            steps{
                 git credentialsId: 'da4e983b-7a53-4496-af74-88d0b1caf091', url: 'https://github.com/mukulchh/sampleprogram'
            }
                
        }
        stage("Maven Build"){
            steps{
                 sh "mvn clean package"
            }
                
        }
        
    }
    
}
