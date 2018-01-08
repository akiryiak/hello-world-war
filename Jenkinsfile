node {
  stage('Build') {
    git 'https://github.com/akiryiak/hello-world-war.git'
    mvnHome = tool 'M3'
    sh '${mvnHome}/bin/mvn clean install'
  }
  stage('Test') {
    junit '**/target/surefire-reports/TEST-*.xml'
    archive 'target/*.jar'
  }
}
