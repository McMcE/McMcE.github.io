<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <meta property="og:url" content="https://www.uk.emb-japan.go.jp/en/quiz/cats.html" />
        <meta property="og:title" content="Cats in Japan" />
        <meta property="og:description" content="How much do you know about cats in Japan?" />
        <meta property="og:image" content="http://www.uk.emb-japan.go.jp/en/invi/EoJ Logo (white background).png" />
        <title>Quiz: Cats in Japan</title>
        <link href="https://fonts.googleapis.com/css?family=Roboto+Condensed|Material+Icons" rel="stylesheet" type="text/css">
        <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.9.0/css/all.min.css" rel="stylesheet" type="text/css">
        <link href="lib/css/quiz_centered.css" rel="stylesheet" type="text/css">
    </head>

    <body>
        <div id="quiz_container"></div>
        <div id="fb-root"></div>
		<script async defer crossorigin="anonymous" src="https://connect.facebook.net/en_GB/sdk.js#xfbml=1&version=v7.0"></script>
        <script src="lib/js/jquery.js"></script>
        <script src="lib/js/jquery.easing.1.3.js"></script>
        <script src="lib/js/jquery.transit.min.js"></script>
        <script src="lib/js/essemble_core.min.js"></script>
        <script src="lib/js/mcq.js"></script>
        <script src="lib/js/quiz.js"></script>
        
        <script>
        var quiz;

        function init(){
            
            //create the screen object which loads the xml and creates all screen elements
            quiz = new Screen({id:"myQuiz", xmlPath:"lib/xml/cats.xml"});
            
            //choose a target div
            var targetDiv = get("quiz_container");
            
            //load it
            quiz.load(targetDiv,false);
        }
        
        //kick off
        $(document).ready(function() {
            init();
                   
        });
                
        </script>

    </body>
</html>

