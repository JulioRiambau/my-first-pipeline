pipeline {
    agent { node { label 'windows' }  }
    stages {
        stage('test') {
            steps{
                echo 'Starting Ranorex test'

                script{
                    def returnStatus = bat(
                        label: "Run Ranorex test",
                        script: "C:\\Work\\Projects\\Ranorex\\CassandraMigration\\CassandraMigration\\bin\\Debug\\CassandraMigration.exe",
                        returnStatus: true)

                    if (returnStatus == 0) 
                    {
                        println("Ranorex test executed successfully.")
                    } 
                    else 
                    {
                        println("Ranorex test failed to execute.")
                    }
                } 
            }
        }
    }
}
