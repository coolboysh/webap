pipeline {
  agent any
  tools {
    maven 'MAVEN'
  }
   stages {
    stage ('Initialize') {
      steps {
        sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
            ''' 
      }
    }
     
     stage ('Build') {
       steps { 
         sh 'mvn clean package'
     }
     } 
   
   }
}
