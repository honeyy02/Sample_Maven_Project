pipeline{
    agent any
     tools {
        maven 'MAVEN3' // Use the name you gave in the Global Tool Configuration
    }
    stages{
        stage('Build'){
            steps{
                sh 'mvn clean package'
            }
        }
        stage('Test'){
            steps{
                sh 'mvn test'
            }
            post{
                always{
                    junit 'target/surefire-reports/*.xml'
                }
            }
        }
    }
}