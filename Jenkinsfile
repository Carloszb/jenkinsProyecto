pipeline {
    agent any

    stages {
        stage('Compilar (Build)') {
            steps {
                sh 'mvn clean package'
            }
        }
        
        stage('Desplegar en Tomcat (Deploy)') {
            steps {
                sh 'cp target/*.war /var/lib/tomcat10/webapps/jenkinsProyecto.war'
            }
        }
    }
}