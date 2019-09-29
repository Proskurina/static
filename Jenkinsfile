pipeline {
	agent any
	stages {
		stage('"Upload to AWS"') {
			steps{
				withAWS(region:'eu-west-2',credentials:'aws-static') {
	                s3Upload(bucket:"static-proskurina", file:'index.html', path:'');
	            }
			}
		}
	}
}