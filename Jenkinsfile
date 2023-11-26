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
			stage ("on slave-1") {
                agent {
                    label {
                       label "dev"
                       customWorkspace "/mnt/velo-app1"
                    }
                }
                steps {
				            sh "sudo git clone https://github.com/shubham51294/velo-app.git -b 2023Q1"
                    sh "sudo cp -r index.html /var/www/html"
                    sh "sudo chmod -R 777 /var/www/html/index.html"
                    }
                }
            stage ("on slave-2") {
                agent {
                    label {
                       label "qa"
                       customWorkspace "/mnt/velo-app2"
                    }
                }
                steps {
				            sh "sudo git clone https://github.com/shubham51294/velo-app.git -b 2023Q2"
                    sh "sudo cp -r index.html /var/www/html"
                    sh "sudo chmod -R 777 /var/www/html/index.html"
                    }
                }
           	stage ("on slave-3") {
                agent {
                    label {
                       label "vir"
                       customWorkspace "/mnt/velo-app3"
                    }
                }
                steps {
				            sh "sudo git clone https://github.com/shubham51294/velo-app.git -b 2023Q3"
                    sh "sudo cp -r index.html /var/www/html"
                    sh "sudo chmod -R 777 /var/www/html/index.html"
                    }
                }
            }
}			
			
