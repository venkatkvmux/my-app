
node {
  stage('SCM checkout'){
    git 'https://github.com/venkatkvmux/my-app'
  }
  stage('Compile-package'){
    def mvnhome = tool name: 'maven-3', type: 'maven'
    sh "${mvnhome}/bin/mvn package"
  }
  stage('email notification'){
    mail bcc: '', body: 'Welcome to Jenkins', cc: '', from: '', replyTo: '', subject: 'Jenkins job', to: 'venkat.m.kanna3@gmail.com'
  }
}

