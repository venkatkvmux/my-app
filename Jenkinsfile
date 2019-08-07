
node {
  stage('SCM checkout'){
    git 'https://github.com/venkatkvmux/my-app'
  }
  stage('Compile-package'){
    def mvnhome = tool name: 'maven-3', type: 'maven'
    sh "${mvnhome}/bin/mvn package"
  }
}

