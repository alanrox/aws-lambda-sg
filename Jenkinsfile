def bucket = 'repo-ost'
def functionName = 'lambda-sg'
def region = 'us-east-1'

node('slaves'){
    stage('Checkout'){
        checkout scm
    }

    stage('Test'){
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
