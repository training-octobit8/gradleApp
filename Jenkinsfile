node {
  stage('SCM') {
    sh "git clone https://github.com/training-octobit8/gradleApp.git"
  }
  stage('SonarQube Analysis') {
    withSonarQubeEnv() {
      sh "./gradlew sonarqube"
    }
  }
}
