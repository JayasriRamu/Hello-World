node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    def mvn = tool 'Default Maven';
    withSonarQubeEnv() {
     bat "${mvn}/bin/mvn clean verify sonar:sonar -Dsonar.projectKey=Sonar-first-test"
    }
  }
}

// node {
//   environment {
//      env.PATH = env.PATH + ";c:\\Windows\\System32"
//  }
//   stage('SonarQube analysis') {
//     def scannerHome = tool name: 'SonarQubeScanner';
//     withSonarQubeEnv('localsonar') { 
//       bat "${scannerHome}/bin/sonar-scanner"
//     }
//   }
// }

