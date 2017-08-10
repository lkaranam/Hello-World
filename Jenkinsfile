node('master') {
    stage('Build') {
        "echo Build"
    }
    stage('Test'){
      parallel (
        "JUnit": { 
            "echo JUnit"
        },
        "DBUnit": { 
            "echo DBUnit"
        },
        "Jasmine": { 
            "echo Jasmine"
        },
      )
    }
    stage('Browser Tests'){
      parallel (
        "Firefox": { 
            "echo Firefox"
        },
        "Edge": { 
             "echo Edge"
        },
        "Safari": { 
             "echo Safari"
        },
        "Chrome": { 
             "echo Chrome"
        },
      )
    }
    stage('Dev'){
        "echo Dev"
    }
    stage('Staging'){
        "echo Staging"
    }
    stage('Production'){
        "echo Production"
    }
}
