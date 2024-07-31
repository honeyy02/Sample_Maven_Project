pipeline{
    agent any
     tools {
        maven 'MAVEN3' // Use the name you gave in the Global Tool Configuration
    }
    stages{
        stage('Build'){
            steps{
                sh 'mvn -B -DskipTests clean package'
            }
        }
        stage('Archive'){
            steps{
                archiveArtifacts artifacts: 'target/*.jar', followSymlinks: false
            }
        }
        stage('Test'){
            steps{
                sh 'mvn test'
            }
            
        }
    }
}
