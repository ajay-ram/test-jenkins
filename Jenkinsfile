pipeline{
  agent any
  stages{
    stage ('one'){
      steps{
        echo 'stage 1 running'
      }
    }
    stage ('two'){
      steps{
        input ('do you want to proceed?')
      }
    }
    stage ('three'){
      when{
        not{
          branch 'master'
        }
      }
      steps{
        echo 'hello'
      }
    }
  }
}
