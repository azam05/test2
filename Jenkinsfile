pipeline {
    agent { label 'master' }
    stages {
       stage('build') {
          steps {
             bat 'C:\\Axway-7.5.3\\apigateway\\Win32/bin\\projpack.bat --create --dir=C:\\projets\\API_Management\\Team_Development\\apipackages --type fed --name=Asim_UAT_Team_Dev_Fed_Package --add C:\\Users\\Asim\\apiprojects\\test --projpass-none --passphrase-none'
          }
       }
    }
}