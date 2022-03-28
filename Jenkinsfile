node {
    stage("Clone"){
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/aidagaiti/VPC_Deployer.git']]])
    }
    stage("Build"){
        sh "docker build -t VPC_Deployer . "
    }
}