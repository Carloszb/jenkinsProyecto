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
                sh 'cp target/mi-app.war /var/lib/tomcat10/webapps/mi-app.war'
            }
        }
    }
}