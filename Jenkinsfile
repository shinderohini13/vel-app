pipeline {

    agent any 
	
	stages {
	
	   stage ('install apache') {
	   
	      steps {
		  
		      sh "sudo yum install httpd -y"
		  }
	   
	   }
	   stage ('start apache') {
	   
	      steps {
		  
		      sh "sudo service httpd start"
		  
		  }
	   
	   }
	   stage ('deploy index') {
	   
	      steps {
		  
		      sh "cp index.html /var/www/html/"
			  sh "chmod -R 777 /var/www/html/index.html"
		  
		  }
	   
	   }
	
	
	}

}
