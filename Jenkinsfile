pipeline {
    agent any 
    stages{
       stage(message){
         steps {
             echo "This is parallel Job"
         }
       
       }
       stage('imagebuild'){
           steps {
              parallel test1: {
                sh '''
                    echo "This is test1"
                '''
},
              test2: {
                sh '''
                   echo "This is test2"
                   echo "$WORKSPACE"
                '''

}
           }
       
       }
       stage(clone){
           steps{
               echo "test"
       }
       }
    
    }


}
