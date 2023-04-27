pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       maven 'maven' 
    }
    

    stages{
        stage('Build'){
            steps{
                echo 'this is the build job'
                sh 'mvn compile'
            }
        }
        stage('test'){
            steps{
                echo 'this is the second job'
                sh 'mvn test'
            }
        }
        stage('package'){
            steps{
                echo 'this is the third job'
                sh 'mvn package'
                sleep 7
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed for shopping-potal app...'
        }
        
    }
    
}
