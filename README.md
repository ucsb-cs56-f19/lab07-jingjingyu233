
Javadoc: https://ucsb-cs56-f19.github.io/lab07-jingjingyu233/

Heroku: https://cs56-f19-lab07-jingjingyu233.herokuapp.com

Github: https://github.com/ucsb-cs56-f19/lab07-jingjingyu233 Running on Localhost.

A simple Spring Boot webapp using:

    Thymeleaf templating
    Pulling in Bootstrap from CDN.
    Github OAuth

    You must first configure a GitHub OAuth app for http://localhost:8080 and obtain the client-id and client-secret.

    Follow the instructions here: https://ucsb-cs56.github.io/topics/oauth_github_setup.
        For the application url, use http://localhost:8080
        For the callback url, also use http://localhost:8080
        Note that on localhost, you typically need use http not https

    You must then copy the file localhost.json.SAMPLE to the file localhost.json.
        Note that you SHOULD NOT edit localhost.json.SAMPLE directly.
        The copied file localhost.json will NOT be commited to GitHub; it's in the .gitignore

    Then, edit the localhost.json file and put in your client id and client secret in the places indicated.

    Finally, IN EACH terminal session where you are going to run mvn spring-boot:run, and EACH TIME after you change the values in localhost.json, execute this command to load those values into the Unix environment:

    . env.sh

    That's a dot followed by a space followed by env.sh, not a typo. That means to source the contents of env.sh into the current shell. That loads the contents of localhost.json into the environment variable SPRING_APPLICATION_JSON, which causes those values to override those in the application.properties file.

    Now you are ready to do mvn spring-boot:run as usual, and see the application on http://localhost:8080.

    Try logging in with your GitHub account.

