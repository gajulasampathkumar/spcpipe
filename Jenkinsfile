node
{

 stage('SCM')
  {
   git 'https://github.com/gajulasampathkumar/spcpipe.git'
  }
 stage('build and package')
  {
   sh 'mvn clean package'
  }
 stage('arachive the artifacts')
  {
    archive 'target/*.jar'
  }
 stage('showing test result')
  {
   junit 'target/surefire-reports/*.xml'
  }

}