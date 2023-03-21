node {
  environment {
     env.PATH = env.PATH + ";c:\\Windows\\System32"
 }
  stage('SonarQube analysis') {
    def scannerHome = tool name: 'SonarQubeScanner';
    withSonarQubeEnv('localsonar') { 
      bat "${scannerHome}/bin/sonar-scanner"
    }
  }
}

