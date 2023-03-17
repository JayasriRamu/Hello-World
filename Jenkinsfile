node {
  stage('SonarQube analysis') {
    def scannerHome = tool name: 'sonarScanner', type: 'hudson.plugins.sonar.SonarRunnerInstallation';
    withSonarQubeEnv('SonarQube') { 
      sh "${scannerHome}/bin/sonar-scanner"
    }
  }
}

