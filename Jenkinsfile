node {
    stage('Clone Repository') {
        git  branch: 'main', url:'https://github.com/ryuzaki710/Rohiot-demo.git'
    }
	
  stage('Upload to S3') {
        sh '''
        aws s3 cp .	 s3://rohit-travel-demo-website/ --recursive
        '''
    }
}
