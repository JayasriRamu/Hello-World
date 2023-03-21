node {
  stage('SonarQube analysis') {
    def scannerHome = tool name: 'SonarScanner', type: 'hudson.plugins.sonar.SonarRunnerInstallation';
    withSonarQubeEnv('localsonar') { 
      sh "${scannerHome}/bin/sonar-scanner"
    }
  }
}

