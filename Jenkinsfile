node {
  stage('SonarQube analysis') {
    def scannerHome = tool name: 'SonarScanner', type: 'hudson.plugins.sonar.SonarRunnerInstallation';
    withSonarQubeEnv('SonarQube') { 
      sh "${scannerHome}/bin/sonar-scanner"
    }
  }
}

