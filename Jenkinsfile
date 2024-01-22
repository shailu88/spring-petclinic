node('JDK8'){
        stage('sourcecod checkout'){
          git branch: 'main', url: 'https://github.com/shailu88/spring-petclinic.git'
          }
        stage('Bild the code'){
          sh 'mvn clean package'
          }
        stage('Archving results'){
          junit '**/surefire-reports/*.xml'
          archive '**/target/*.jar'
          }
}
