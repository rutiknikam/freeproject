pipeline{
  options {
          buildDiscarder(logRotator(numToKeepStr: '5', artifactNumToKeepStr:'5'))
  }
   agent any
        tools{maven 'maven' }
      stages{
         stage('code compilation'){
           Steps{
                sh 'mvn clean compile'
                 }
            }
            stage('code packaging'){
                       Steps{
                            sh 'mvn clean package'
                             }
                        }
      }
}
