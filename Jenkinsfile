pipeline{
  agent{
    label('node1')

  }
    stages{
    stage('stage-1'){
      steps{
        sh "mkdir /mnt/gol1"
        sh "git clone https://github.com/yogitatupke/game-of-life.git /mnt/gol1"
        sh "cd /mnt/gol1/"
        sh "mvn clean install -DskipTests=true"
        sh "cp -r gameoflife-web/target/gameoflife.war /mnt/servers/apache-tomcat-9.0.76/webapps/"
        
        
        
      }
    }
    }
      
  }
