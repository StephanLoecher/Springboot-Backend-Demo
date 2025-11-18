pipeline{
  agent any
  stages{
      stage("A"){
      steps{
        echo "Webhook works"
      }      
    }
  }
  post{
    always{
      echo "========always========"
    }
    success{
      echo "========pipeline executed successfully ========"
    }
    failure{
      echo "========pipeline execution failed========"
    }
  }
}