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
           git clone "https://gitlab.com/dev_lx/ansible_projects.git"
           sh "ls"
       }

    
    }


}
