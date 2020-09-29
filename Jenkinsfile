pipeline{
    agent any
    
    enviornment{
        PATH="${PATH}"
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
