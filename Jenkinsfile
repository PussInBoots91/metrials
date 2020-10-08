pipeline {
    agent any
    environment {
        PATH = "/opt/maven/bin/:$PATH"
    }
    stages {
        stage ("clone code"){

            steps{
                git credentialsId: 'PussInBoots91', url: 'https://github.com/PussInBoots91/metrials.git'
            }
        }
        stage("Build Code")
         steps{
             sh "mvn clean install"
         }
    }
}
