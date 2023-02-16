pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        sh 'g++ -o task5 task5_code.cpp'
        build job: 'PES1UG20CS204-1'
      }
    }
    stage('Test'){
      steps{
        sh './task5'
      }
    }
  }
  post{
    failure{
      echo 'Pipeline failed'
    }
  }
}
