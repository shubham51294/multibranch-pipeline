pipeline {
     agent {
	     label {
		     label "qa"
			 customWorkspace "/mnt/velocity2"
			 }
		}
        stages { 
            stage ("on slave-2") {
                 steps {
	             sh "sudo git clone https://github.com/shubham51294/velo-app.git -b 2023Q2"
                     sh "sudo cp -r index.html /var/www/html"
                     sh "sudo chmod -R 777 /var/www/html/index.html"
                       }
                }
	}
}	
