pipeline{
  agent any
  
  stages{
    stage('Build'){
      steps {
        sh 'g++ -o PES1UG20CS358-1 brandnewfile.cpp'
      }
    }
    
    stage('Test'){
      steps {
        sh './PES1UG20CS358-1'
      }
    }
    
    stage('Deploy') {
      steps{
        echo 'Deployment Successful'
      }
    }
  }
  
  post{
    success{
      echo 'Pipeline Finished'
    }
    
    failure{
      echo 'Pipeline Failed'
    }
  }
}
