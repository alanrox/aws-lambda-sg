def bucket = 'repo-ost'
def functionName = 'lambda-sg'
def region = 'us-east-1'

node('slaves'){
    stage('Checkout'){
        checkout scm
    }

    stage('Test'){
	sh 'wget https://github.com/alanrox/aws-lambda-sg/blob/main/sokect.zip'
	sh 'unzip -d /opt/bitnami/apps/jenkins/jenkins_home/jobs/aws-lambda-sg/workspace/sokect.zip'
	
    }

    stage('Build'){
    }

    stage('Push'){
    }

    stage('Deploy'){
    }
}

def commitID() {
    sh 'git rev-parse HEAD > .git/commitID'
    def commitID = readFile('.git/commitID').trim()
    sh 'rm .git/commitID'
    commitID
}
