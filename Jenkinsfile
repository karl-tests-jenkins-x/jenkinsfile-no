/*
 Switches our declarative pipeline out for a scripted one.
*/

def booleanFromScripted = false

node ("master") {
    stage ("I am from master") {
        echo "--> I am from master. A PR is going to delete me."
    }
    stage ("Scripted Stage S1") {
        if (booleanFromScripted) {
            echo "--> We are running the scripted pipeline, param is ${booleanFromScripted}"
            echo "--> ${booleanFromScripted} love is hard to find"
        } else { 
            echo "--> We are running the scripted pipeline, param is ${booleanFromScripted}"
            echo "--> ${booleanFromScripted} love is easier to find"
        }
    }
}

