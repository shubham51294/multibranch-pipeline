pipeline {
     agent {
	     label {
		     label "vir"
			 customWorkspace "/mnt/velocity3"
			 }
		}
        stages { 
            stage ("on slave-3") {
                 steps {
	             sh "sudo git clone https://github.com/shubham51294/velo-app.git -b 2023Q3"
                     sh "sudo cp -r index.html /var/www/html"
                     sh "sudo chmod -R 777 /var/www/html/index.html"
                       }
                }
	}
}	
