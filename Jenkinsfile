pipeline{
 agent any
  stages{
    stage(checkout){
     steps{
        checkout SCM
          }
      }
    stage(build){
     steps{
        sh 'mvn install'
       }
      }
    stage(deployment){
     steps{
        sh 'cp target/pipelinerepo1.war /home/nikita/Documents/devops/apache-tomcat-9.0.93/webapps'
     }
  }
 }
}
