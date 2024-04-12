pipeline { 
  agent any
  tools { 
    gradle "Gradle 8.7"
  }
  stages { 
    stage('clone repository') {
      steps { 
        git 'https://github.com/beniye19/java-todo.git'
      }
    }
    stage('Build the project') {
      steps { 
        sh 'gradle build'
      }
    }
    stage('Tests') {
      steps { 
        sh 'gradle test'
      }
    }
  }
}

