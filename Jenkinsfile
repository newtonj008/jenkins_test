// Allocate Build Node
node('master') {
    stage("Fetch Source Code") {
        git 'https://github.com/newtonj008/Jenkins_test/'
    }

    dir('Lesson5') {
        printMessage('Running Pipeline')

        stage("Testing") {
            sh '/usr/bin/python2 test_functions.py'
        }

        printMessage('Pipeline Complete')
    }
}

def printMessage(message) {
    echo "${message}"
}
