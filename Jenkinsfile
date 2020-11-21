pipeline{
    agent any
    
    triggers {
        pollSCM '* * * * *'
    }
    
    stages{
        stage("Build"){
            steps{
               sh 'mvn -B -DskipTests clean package'
            }
        }
    }
    
}