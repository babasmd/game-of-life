node{
   stage('SCM')
{     
git 'https://github.com/babasmd/game-of-life.git'

}
   
 stage('build & Package')
{
            sh 'mvn package'
    
}    

    stage('results')
{
        archive 'gameoflife-web/target/gameoflife.war'
        junit 'gameoflife-web/target/surefire-reports/*.xml'

    
}

}