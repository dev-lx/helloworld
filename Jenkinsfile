pipeline {
    agent any 
    stages{
       stage(message){
         steps {
             echo "This dev"
         }
       
       }
       stage(message2){
           steps {
              echo "dev completed"
           }
       
       }
       stage(clone){
           steps{
               git clone "https://github.com/dev-lx/helloworld.git"
               sh "ls"
       }
       }
    
    }


}
