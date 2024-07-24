pipeline{
    agent any
     tools {
        maven 'MAVEN3 3.9.8' // Use the name you gave in the Global Tool Configuration
    }
    stages{
        stage('Build'){
            steps{
                sh 'mvn clean package'
            }
        }
    }
}