pipeline{
    agent any
    stages{
        stage('gradle build stage'){
            steps{
                sh './gradlew build --no-daemon'
            }
        }
        stage('artifacts'){
            steps{
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
