pipeline{
  agent any
  tools{
    maven 'Maven'
  }
  stages{
      stage("Cleanup"){
      steps{
        sh "mvn --version"
        sh "mvn compile"
      }      
    }
  }
  post{
    always{
      echo "Always is running"
    }
    success{
      echo "========pipeline executed successfully ========"
    }
    failure{
      echo "========pipeline execution failed========"
    }
  }
}