pipeline {
            agent {
               
                label {
                          label ('built-in')
                          customWorkspace ('/mnt/multibranch/')
                       }
                 }
         
         stages {
             stage ('git-clone'){
         
                              steps{
                                 
                                 sh "rm -rf *"         
                                 sh "git clone https://github.com/shahidshaikh962311/test-application.git"
                                  
                                   }
                             }
               
             stage ('deploy'){
        
                          steps{
           
                                 sh "cp -r /mnt/multibranch/index.html /var/www/html/"
                                 sh "chmod -R 777 /var/www/html"
                             }
                    
                      }

               }

       }
