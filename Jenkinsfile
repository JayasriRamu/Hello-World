node {
  stage('SonarQube analysis') {
    def scannerHome = tool name: 'SonarQubeScanner', type: 'hudson.plugins.sonar.SonarRunnerInstallation';
    withSonarQubeEnv('localsonar') { 
      sh "${scannerHome}/bin/sonar-scanner"
    }
  }
}

