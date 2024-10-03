This is my attempt to be organized

Class Start
    PROF VENTURA SECTION 003
        served mission in Sendai, Japan
        researches AI specifically Computational Creativity (what does it mean to be creative, AI is not. Just makes stuff)

        AWS account, Introduction assignment, and Discord Assignment by Saturday 11:59

        What is web programming?
            HTML
                what it is that you have (structure)
            CSS
                makes it look pretty (cosmetics)
            Javascript
                gives it functionality (what it does)

            we'll use codepen.io to use all three in tandem

            need to collaborate, curiosity, creativity, and expertise - Tim Cook

        Course Objectives
            learn to love learning
            Gain confidence - imposter syndrome is real, you are ok
            Have fun - physics sucks, but it's still interesting and fun. If you don't know what the answer is, have fun with it
            Learn web programming

        CS260 zoom out view
            Use a bunch of new things to build new things in different things

            27 little homeworks
            1 BIG project (startup), broken into several pieces
                #Construction Estimating Software
                #Fake NASA C.A.P.E page - fun space fact playground / launchpad for C.A.P.E shirts
                Can submit to Demo Day on Dec 7: 10 people, 5 min presentation of your web app to the class
            2 exams (check-ups on how we're doing)

        How we interact
            Class 2x a week + TA help in various places (TlMG, Discord*, etc.)
            Course content ALL on GitHub (rendered through Canvas)
            Submit assignments and check grades on Canvas (launchpad for class)
                checkmark = assignment due Saturday
                rocket-ship = SUPER IMPORTANT deliverable due date (part of startup project)

        NOTES
            development machine (laptop fine)
            $50 for AWS, credits available
            Focus on mastery instead of grades
            9-10 hours per week <---- Hard class, but worth it
            Patience (Don't be trapped by the accumulation of ignorance, understand everything as you go) (don't skip stuff)
            learn how to learn
            turn stuff in on time
            teamwork is amazing
            ask questions, it sucks but do it to:
                1. yourself
                2. google (if use AI, double check it)
                3. peers
                4. TA
                5. instructor
            VALUE YOUR OPPORTUNITY:
                "Education means emancipation. It means light and liberty.
                It means the uplifting of the soul of man into the glorious
                light of truth, the light by which men can only be made free."
                    - Frederick Douglas

9.10
    STARTUP
        Parts - THINGS YOU NEED IN YOUR STARTUP TO GET CREDIT
            Startup cool idea - balance it with reality, have to be done with A VERSION of it by the end of the semester - keep moving forward
                something space / stars
                CAPE launchpad / NASA imitation
                some form of construction estimating software
                a game / interactive story of the Sequel / DND
                bowling stats app that helps you bowl better, take info on bowling balls from company pages, pick coaches brain for more stuff
            HTML - Structure
            CSS - Style
            JavaScript - Interaction
            React - Web Framework
            Service - Web service endpoints
            Database - Persisted data
            Login - Authentication
            WebSocket - Data pushed from server, chat
        What we're going to do with it
            Clone deliverable repository
            Play with it
            Debug it in dev space
            Release it on web

        Server
            has all the data
        Client
            makes request to the server for data

        Pier to Pier
            client doesn't have to request from server to request from other client
            two clients communicate directly
            ie. chess game


        GET VS CODE AND USE IT
            Need it for this class, look into switching to it for cs235 as well

        Make sure to do ALL your coding / debugging in your development software
            THEN you push what you're happy with to Production software
            AND / OR save to GitHub repository

9.12
    GIT
        Commit often
            Git commits MUST represent all work
        Don't use large binary files
        Don't put sensitive information there

        Play around with SIMON
            break it/fix it/use it as a model for your start up
        development environment
            the place where all the coding and play happens on your local device
        production environment
            the place in the cloud where the "perfect version" of your startup is

9.19
    SIMON HTML
        https://simon.yourdomain
        |
        |
        index.html   about.html   scores.html   other.html     //hyperlinks direct to each individual html page



        popups in web page = separate page in html or button clicked shows a jpeg of popout

        FORMAT
            index.html > html > head > body > header > main > footer
            - tells system it is html >
            - actual html code >
            - head tells system what to do/not to do with certain things (like saying I'll resize for mobile, don't do it automatically cause your bad at it) >
            - normally has a header, main, and footer >
            - same on all pages >
            -  >
            - same on all pages >

9.24
    CSS: RULES, BOX MODEL, FONTS, ANIMATIONS

        One way to think about a websocket is pushing to the user without them having to pull it
            ex: pushing player updates


        CSS Rules:
            CSS = Cascading Style Sheets
            the closest child takes precedence over a parent with a similarly styled rule
                if body is red, paragraph is green, and span is purple in CSS, the most specific one wins in it's particular instance
            rules either go in individual html selector, in html header, or in separate file
                precedence occurs in that order.

            rules point to an html, a selector in the html(p), a property(color), declaration(:), and value(green)
                p{color:green}
                will turn all text in paragraphs green

            add a link to a CSS sheet that includes all the rules (better way to do the above)
                <head>
                <link rel="stylesheet" href="styles.css" />
                </head>
                        styles.css FILE:
                        p {
                            color:green
                        }

            many ways to make a CSS rule selective and not all inclusive, giving different class names or n'th child are two of them

            SELECTORS
                element: all elements of a specific name (ex: div); any div element
                ID: The element with the given ID; (ex: #root); The element with the attribute id='root'
                Class: ALl elements with the given class (ex: .highlight); Any element with the attribute class='highlight'
                element class: Any elements with the specific name and class (ex: p.highlight); Any p element with the attribute class ='highlight'
                List: Any of the given selectors (ex: body,section); Body or section elements
                Descendant: A list of descendants (ex: body section); Any section that is a descendant of a body
                Child: A list of dire
                Pseudo: state based (ex: p:hover); The mouse is hovering over a paragraph element

            CSS WEBSITES: W3Schools.com or MDNWebDocs

            WHEN IN A CSS FILE
                you don't need brackets for statements as long as you indent properly
                you only need a semi-colon at the END of the rule
        Box Model:
            everything on your page is a box
                everything in an element is at the center of the box of that specific element
                each box has padding around the content of an element box which can be manipulated in CSS
                element boxes have borders which can be changed in CSS
                margin is space between the padding and the border that no other element box can infringe on


        CSS Fonts:
            Important not to have to many different fonts


        CSS Animation:
            Start small and grow big over 3 seconds. Very end it gets a little bigger than max size and settles back at max size
                p {
                    text-align: center;
                    font-size: 20vh;

                    animation-name: demo;
                    animation-duration: 3s;
                }

            @keyframes demo {
                from {
                    font-size: 0vh;
                }
                95% {
                    font-size: 21vh;
                }
                to {
                font-size: 20vh;
                }
            }

9.26
    WAYS TO ALTER THE DISPLAY
        Block
            selector fills whole display
        Inline
            only as big as selector is
        Grid
            put stuff in a grid
        Flex
            Grid but fancy
        Media Queries
            a way to ask the screen what it is doing and do stuff to it
        Float

10.03
    JAVASCRIPT
        Adding JS to HTML
            sort of same way we hook CSS to HTML
            3 ways
                In the head (script file)
                In the body (script tag)
                    <script>
                        code here
                    </script>
                In the footing (script attribute)
                    <button onclick="sayHello()">Say hello</button>
                        when clicking the button, the sayHello function will run from the JS file
