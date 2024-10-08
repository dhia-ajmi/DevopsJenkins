pipeline {

    agent any

    tools {
        jdk 'jdk-17'         // Remplacez par le nom du JDK configuré dans Jenkins
        maven 'maven-3'      // Remplacez par le nom de Maven configuré dans Jenkins
    }

    stages {

        stage('GIT') {

            steps {

                git branch: 'master', url: 'https://github.com/dhia-ajmi/DevopsJenkins.git'

            }

        }

        stage('Compile Stage') {

            steps {

                sh 'mvn clean compile'

            }

        }

    }

}
