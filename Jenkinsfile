pipeline {
    agent any

    stages {
    stage('Clone source code') {
        scmVars = checkout scm
        // scmVars contains the following values
        // GIT_BRANCH=origin/mybranch
        // GIT_COMMIT=fc8279a107ebaf806f2e310fce15a7a54238eb71
        // GIT_PREVIOUS_COMMIT=6f2e319a1fc82707ebaf800fce15a7a54238eb71
        // GIT_PREVIOUS_SUCCESSFUL_COMMIT=310fce159a1fc82707ebaf806f2ea7a54238eb71
        // GIT_URL=https://stash.someworkplace.com/scm/poc/api-sample.git
    }
    stage('test scope') {
      echo scmVars.GIT_BRANCH
    }
    }
}
