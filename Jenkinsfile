pipeline {
  agent {
    dockerfile {
      filename 'dockerfile'
    }

  }
  stages {
    stage('compile') {
      steps {
        git(url: 'https://gitlab.com/wiga-nlp/nebula-middleware.git', branch: 'master', credentialsId: 'chandra.jakhar@gmail.com', poll: true, changelog: true)
        gitlabBuilds()
      }
    }

  }
}