pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        sh 'g++ -o newtask5 task5_new218.cpp'
        build job: 'PES1UG20CS218-1'
      }
    }
    stage('Test'){
      steps{
        sh './newtask5'
      }
    }
   stage('Deploy'){
      steps{
        echo 'Deploying'

      }
    }
  }
  post{
    failure{
      echo 'Pipeline failed'
    }
  }
}
