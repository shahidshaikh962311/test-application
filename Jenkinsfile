pipeline {
            agent {
               
                label {
                          label ('172.31.37.70')
                          customWorkspace ('/mnt/multibranch/')
                       }
                 }
         
         stages {
             stage ('git-clone'){
         
                              steps{
                                 
                                 sh "rm -rf *"         
                                 sh "git clone https://github.com/shahidshaikh962311/test-application.git -b branch-2"
                                  
                                   }
                             }
               
             stage ('deploy'){
        
                          steps{
           
                                 sh "cp -r /mnt/multibranch/test-application/index.html /var/www/html/"
                                 
                             }
                    
                      }

               }

       }
