pipeline{
    agent any
     tools {
        maven 'Maven3 3.6.3' // Use the name you gave in the Global Tool Configuration
    }
    stages{
        stage('Build'){
            steps{
                sh 'mvn clean package'
            }
        }
    }
}