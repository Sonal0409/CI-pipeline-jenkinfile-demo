pipeline{
    
    agent any
    
    tools{
        maven 'mymaven'
    }
    
    stages{
        stage('Checkout Code')
        {
            steps{
                git 'https://github.com/Sonal0409/DevOpsCodeDemo.git'
            }
        }
        
        stage('ComplileCode'){
            steps{
                sh 'mvn compile'
            }
        }
        
        stage('Test Code'){
            steps{
                sh 'mvn test'
            }
        }
        
        stage('Build Code'){
            steps{
                sh 'mvn clean install package'
            }
        }
    }
    
}
