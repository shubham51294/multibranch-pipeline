pipeline {
     agent {
	     label {
		     label "built-in"
			 customWorkspace "/mnt/velo-app"
			 }
		}
        stages { 
            stage ("one") {
                 steps {
                     sh "cp -r index.html /var/www/html"
                     sh "chmod -R 777 /var/www/html/index.html"
                       }
                }
	}
}
