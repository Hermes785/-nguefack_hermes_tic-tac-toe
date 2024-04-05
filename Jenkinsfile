pipeline {
    agent any
    
    tools {
        nodejs 'nodejs'
    }
    stages {
        stage('Build') {
            steps {
                echo'Building'
                sh 'npm install'
            }
        }
    stage('Test') {

    steps {
        echo 'Testing'
    }
    } 
    stage('Deploy/Deliver') {
            steps {
                echo 'Deploying'
                sh 'npm run build'
                
            }
            post{
                always{
                    archiveArtifacts artifacts:'build/**/*.*', onlyIfSuccessful:true
                }
            }
        }
    }
}
