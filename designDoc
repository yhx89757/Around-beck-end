main:
    // create index in elasticsearch database
    createIndexIfNotExist()
    // upload posts (image and video) from database and annotate the image posts with google version api
    handlerPost {
        url: "/post"
        method: "POST", "OPTIONS"
    }
    // search posts (image and video) from database
    handlerSearch {
        url: "/search"
        method: "GET", "OPTIONS"
    }
    // filter faces from all over the world by using google vision api
    handlerCluster {
        url: "/cluster"
        method: "GET", "OPTIONS"
    }

user:
    // register user
    handlerSignup {
        url: "/signup"
        method: "POST", "OPTIONS"
    }
    // login user and generate and send back the token string to the front end
    handlerLogin {
        url: "/login"
        method: "POST", "OPTIONS"
    }
vision:
    // use google vision api to detect face and return the score
    annotate {}
