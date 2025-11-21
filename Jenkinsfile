pipeline{
  agent any
  tools{
    maven 'Maven'
  }
  stages{
      stage("Cleanup"){
      steps{
        sh "mvn dependency:tree"
      }      
    }
  }
  post{
    always{
      echo "mvn clean"
    }
    success{
      echo "========pipeline executed successfully ========"
    }
    failure{
      echo "========pipeline execution failed========"
    }
  }
}