
node {
  stage('SCM checkout'){
    git 'https://github.com/venkatkvmux/my-app'
  }
  stage('Compile-package'){
    sh 'mvn package'
  }
}

