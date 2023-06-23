pipeline{
  options {
          buildDiscarder(logRotator(numToKeepStr: '5', artifactNumToKeepStr:'5'))
  }
   agent any
        tools{maven 'maven' }
      stages{
         stage('code compilation'){
           steps{
                sh 'mvn clean compile'
                 }
            }
            stage('code packaging'){
                       steps{
                            sh 'mvn clean package'
                             }
                        }
      }
}
