node {
  stage('SonarQube analysis') {
    def scannerHome = tool name: 'SonarQubeScanner';
    withSonarQubeEnv('localsonar') { 
      bat "${scannerHome}/bin/sonar-scanner"
    }
  }
}

