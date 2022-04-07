pipeline{
    agent any
    stages{
        stage('gradle build stage'){
            steps{
                sh './gradlew build'
            }
        }
        stage('artifacts'){
            steps{
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}