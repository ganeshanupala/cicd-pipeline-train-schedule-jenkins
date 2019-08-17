pipeline {
    agent any
    stages {
        stage('Build Latest') {
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/mySchedule.zip'
            }
        }
    }
}
