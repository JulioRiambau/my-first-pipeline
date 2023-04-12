pipeline {
    agent { node { label 'windows' }  }
    stages {
        stage('build') {
            steps {
                bat 'C:\Work\Projects\Ranorex\CassandraMigration\CassandraMigration\bin\Debug\CassandraMigration.exe'
            }
        }
    }
}
