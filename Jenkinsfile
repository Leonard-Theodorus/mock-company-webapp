pipeline {
  /*
   * TODO: Implement pipeline stages/steps
   *   See documentation: https://www.jenkins.io/doc/book/pipeline/syntax/#stages
   */
   agent any
   stages{
    stage("stage 1"){
        steps{
            sh "echo $JAVA_HOME"
            echo "${env.JAVA_HOME}"
        }
    }

    stage('Test'){
        steps{
            sh "echo $JAVA_HOME"
            echo "${env.JAVA_HOME}"
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
