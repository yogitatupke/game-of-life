pipeline{
  agent{
    label('built-in')

  }
    stages{
    stage('stage-1'){
      steps{
        sh "mkdir/mnt/gol"
        sh "git clone https://github.com/yogitatupke/game-of-life.git /mnt/gol"
        sh "cd /mnt/gol/"
        sh "mvn clean install -DskipTests=true"
        sh "cp -r gameoflife-web/target/gameoflife.war /mnt/servers/apache-tomcat-9.0.76/webapps/"
        
        
        
      }
    }
    }
      
  }
