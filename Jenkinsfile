pipeline{
  agent any
  stages{
    stage('clone'){
      steps{
        git branch:'main',url:'https://github.com/Rakesh-05-07/calculator.git';
      }
    }
    stage('compile'){
      steps{
        sh'javac Calculator.java'
      }
    }
    stage('build'){
      steps{
        sh'java calculator 25 5'
      }
    }
    stage('test'){
      steps{
        sh'java calculator 30 5'
      }
    }
  }
}
