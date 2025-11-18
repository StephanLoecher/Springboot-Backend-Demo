pipeline{
  agent any
  tools{
    maven 'Maven'
  }
  stages{
      stage("Cleanup"){
      steps{
        sh "mvn --version"
        sh "mvn clean"
      }      
    }
  }
  post{
    always{
      sh "rm -rf ./*"
    }
    success{
      echo "========pipeline executed successfully ========"
    }
    failure{
      echo "========pipeline execution failed========"
    }
  }
}