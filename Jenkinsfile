pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        // Checkout the Git repository
        git 'https://github.com/Grandhicharan/hello-world-war.git'
      }
    } 

    stage('Create Git Tag') {
      steps {
        script {
          def tag = "charan" // Specify the tag name you want to create

          // Create the Git tag
          sh "git tag ${tag}"

          // Push the Git tag to the remote repository
          sh "git push origin ${tag}"
        }
      }
    }
  }
}
