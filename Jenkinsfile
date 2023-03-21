node {
  stage('SonarQube analysis') {
    def scannerHome = tool name: 'SonarQubeScanner';
    withSonarQubeEnv('localsonar') { 
      sh "${scannerHome}/bin/sonar-scanner"
    }
  }
}

