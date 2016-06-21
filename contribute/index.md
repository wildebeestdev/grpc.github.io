---
layout: default
title: Contribute
headline: 'Contribution Guidelines'
bodyclass: contribute
---
<script language="JavaScript">
var forwarding=window.location.hash.replace("#","");
$( document ).ready(function() {
    if(forwarding) {
        console.log(forwarding)
        $("#generalInstructions").hide();
        $("#continueEdit").show();
        $("#continueEditButton").text("Edit " + forwarding);
        $("#continueEditButton").attr("href", "https://github.com/wildebeestdev/grpc.github.io/edit/gh-pages/" + forwarding)
    } else {
        $("#generalInstructions").show();
        $("#continueEdit").hide();
    }
});
</script>

<div class="container markdown">
    <div class="row">
        <div class="col-md-11 nofloat center-block">
            {% include contribute-links.html %}
            <div class="col-sm-8" >
                <p class="lead">To contribute to gRPC documentation, please fork the GitHub gRPC repository and start submiting pull requests.</p>
            </div>
            <div class="col-sm-12">
                <div id="continueEdit">
<div markdown="1">

## Continue your edit

Click the below link to edit the page you were just on. When you are done, press "Commit Changes" at the bottom of the screen. This will create a copy of our site on your GitHub account called a "fork." You can make other changes in your fork after it is created, if you want. When you are ready to send us all your changes, go to the index page for your fork and click "New Pull Request" to let us know about it.

</div>
                    <button class="btn inverse"><a id="continueEditButton"></a></button>

                </div>
                <div id="generalInstructions">
<div markdown="1">

## Edit our site on github

Click the below button to visit the repo for our site. You can then click the "Fork" button in the upper-right area of the screen to create a copy of our site on your GitHub account called a "fork." Make any changes you want in your fork, and when you are ready to send those changes to us, go to the index page for your fork and click "New Pull Request" to let us know about it.

</div>
                    <button class="btn inverse"><a href="https://github.com/wildebeestdev/grpc.github.io/">Browse this site's source code</a></button>

                </div>
            </div>
        </div>
    </div>
</div>