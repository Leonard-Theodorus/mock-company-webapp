pipeline {
  /*
   * TODO: Implement pipeline stages/steps
   *   See documentation: https://www.jenkins.io/doc/book/pipeline/syntax/#stages
   */
   agent any
   stages{
    stage('Test'){
        steps{
            echo "JAVA_HOME: $JAVA_HOME"
            sh './gradlew test'
        }
    }
    stage('Build'){
        steps{
            sh './gradlew assemble'
        }
    }
    
   }
}
