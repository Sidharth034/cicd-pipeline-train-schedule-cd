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
                archiveArtifacts artifacts: '/var/lib/jenkins/workspace/train-schedule_master/dist/trainSchedule.zip'
            }
        }
    }
}
