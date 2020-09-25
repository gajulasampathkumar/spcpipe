node
{

 stage('SCM')
  {
   git https://github.com/gajulasampathkumar/runpipe.git
  }
 stage('build and package')
  {
   sh 'mvn clean package
  }
 stage('arachive the artifacts')
  {
    arachive 'target/.war'
  }
 stage('showing test result')
  {
   junit 'workspace/spcpipe/target/surefire-reports'
  }

}