def inspec_run(){
  sh "inspec exec ./ -t ssh://127.0.0.1"
}
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
  stage('Smoke test DEV'){
    sh "echo 'Smoke tests here'"
  }
  stage('Deploy to QA'){
    sh "echo 'Deploying to QA'"
  }
  stage('Smoke test QA'){
    sh "echo 'Smoke tests here'"
  }
}
