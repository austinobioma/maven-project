pipeline {
   agent any
   stages {

      stage ('Git Checkout') {

         steps {
             git branch: 'main', url: 'https://github.com/austinobioma/maven-project.git'
              }
         }
      stage ('Maven Build') {

         steps {
            sh "cd web && mvn clean package"
            sh " cd web && mvn clean install -DskipTests"
         }
      }
      }

   }