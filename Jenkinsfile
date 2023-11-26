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
	             sh "sudo git clone https://github.com/shubham51294/velo-app.git -b 2023Q1"
                     sh "sudo cp -r index.html /var/www/html"
                     sh "sudo chmod -R 777 /var/www/html/index.html"
                       }
                }
	}
}		
               
       		
			
