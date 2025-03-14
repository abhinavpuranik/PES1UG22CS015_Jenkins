pipeline{
  agent any

  stages{
    stage('Build'){
      steps{
        script{
          sh 'g++ -o program non_existent_file.cpp'

        }
      }
    }
    stage('Test'){
      steps{
        script{
          sh './program'
        }
      }
    }
    stage('Deploy'){
      steps{
        echo 'Deploying the application'
      }
    
  }
}
  post{
    failure{
      echo 'Pipeline failed'
    }
      
  }
}
