pipeline{
  agent{
    label('dev')

  }
    stages{
    stage('stage-1'){
      steps{
        sh "sudo mkdir /mnt/gol2"
        sh "sudo git clone https://github.com/yogitatupke/game-of-life.git /mnt/gol2"
        sh "sudo cd /mnt/gol2/"
        sh "sudo mvn clean install -DskipTests=true"
        sh "sudo cp -r gameoflife-web/target/gameoflife.war /mnt/jenkins/apache-tomcat-9.0.76/webapps/"
        
        
        
      }
    }
    }
      
  }
