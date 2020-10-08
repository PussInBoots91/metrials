Pipeline {
    agent any
    stage {
        stage ('Build Aplication')
          steps {
              sh 'mvn -f metrials/pom.xml clean package'
          }
          post {
              success {
                archiveArtifacts artifacts: '**/*.war'
              }
              
          }
    }

}
