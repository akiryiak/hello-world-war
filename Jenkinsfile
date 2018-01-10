node {
  stage('Build') {
    git 'https://github.com/akiryiak/hello-world-war.git'
    mvnHome = tool 'M3'
    sh "'${mvnHome}/bin/mvn' clean install"
  }
  stage('Test') {
    sh "echo 'Should be some tests here'"
  }
  stage('Publish'){
    sh "echo 'We are publishing artefact to some storage here ...'"
  }
  stage('Deploy to dev'){
    sh "echo 'Deploying to dev'"
  }
  stage('Smoke test'){
    sh "echo 'Smoke tests here'"
  }
}
