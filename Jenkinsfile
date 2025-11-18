pipeline{
  agent any
  tools{
    maven 'Maven'
  }
  stages{
      stage("Cleanup"){
      steps{
        sh "mvn clean"
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