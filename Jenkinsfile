pipeline {
     agent {
	     label {
		     label "dev"
			 customWorkspace "/mnt/velocity1"
			 }
		}
        stages { 
            stage ("two") {
                 steps {
                     sh "cp -r index.html /var/www/html"
                     sh "chmod -R 777 /var/www/html/index.html"
                       }
                }
	}
}		
               
       		
			
