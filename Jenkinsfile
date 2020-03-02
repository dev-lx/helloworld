pipeline {
   agent {
        docker {image 'git:latest'}
 
}
   stages {
        stage('cleanWorkspace'){
            steps{
                step([$class: 'WsCleanup'])
}
}
       stage('clone'){
             steps{
                checkout ([$class: 'GitSCM', branches: [[name: "*/master" ]], userRemoteConfigs: [[url: 'https://github.com/dev-lx/helloworld.git']]])
}
}
       stage('Build') {
           steps {
               script{
                 sh "ls"
                 sh "cat hello.py"
                 sh "python /root/hello.py"

           }
         }
       }
   }
}
