pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo "Running build"
                sh './gradlew build --no-daemon' //it is good for speeding automation on local machines, not on jenkins
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
                
            }
        }
       
        
    }
}
