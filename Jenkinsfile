Pipeline {
    agent any
    stage {
        stage ('Build Aplication')
          steps {
              sh 'mvn clean package'
          }
          post {
              success {
                archiveArtifacts artifacts: '**/*.war'
              }
              
          }
    }

}
