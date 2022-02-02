pipeline
{
    agent any 
    stages
    {
        stage('Build')
        { 
            steps
            {
                bat 'mvn clean install'
            }
        }
        stage('Test')
        { 
            steps
            {
                // 
            }
        }
        stage('Deploy')
        { 
            steps
            {
                bat 'mvn -X -U -V -e -B -DskipTests=true deploy -DmuleDeploy 
                -Dmule.version="4.4.0" -Danypoint.username="omish021996" 
                -Danypoint.password="Lifeb@y2" -Dcloudhub.app="world-timezone" 
                -Dcloudhub.environment="Sandbox" -Dcloudhub.bg="ABC" 
                -Dcloudhub.worker="Micro" -Dregion="us-east-2" -Dworkers="1" 
                -DobjectStoreV2="true"'
            }
        }
    }
}