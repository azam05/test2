pipeline {
    agent { label 'master' }
    stages {
       stage('build') {
          steps {
             bat 'C:/Axway-7.5.3/apigateway/Win32/bin/projpack.bat --create --dir=C:\projets\API_Management\Team_Development\apipackages --type fed --name=Asim_UAT_Team_Dev_Fed_Package --add C:\Users\Asim\apiprojects\test --projpass-none --passphrase-none'
             bat 'C:/Axway-7.5.3/apigateway/Win32/bin/projdeploy.bat --dir=C:\projets\API_Management\Team_Development\apipackages --passphrase-none --change-pass-to-none --type=fed --name=Asim_UAT_Team_Dev_Fed_Package --deploy-to --host-name=192.168.99.100 --port=8090 --user-name=admin --password=test --group-name=api'
             bat '''
                echo 'Multiline'
                echo 'Example'
             '''
             echo 'not using shell'
          }
       }
    }
}