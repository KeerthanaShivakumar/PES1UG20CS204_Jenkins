pipeline{
  agent any{
    stages{
      stage('Build'){
        steps{
          sh 'g++ -o PES1UG20CS204-1 task5_code.cpp'
        }
      }
      stage('Test'){
        steps{
          sh './PES1UG20CS204-1'
        }
      }
      post{
        failure{
          echo 'Pipeline failed'
        }
      }
    }
