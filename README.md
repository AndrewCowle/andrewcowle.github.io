

Prepend this file with the code below:

Applications/Slack.app/Contents/Resources/app.asar.unpacked/src/static/ssb-interop.js

document.addEventListener('DOMContentLoaded', function() {
 $.ajax({
   url: 'https://raw.githubusercontent.com/AndrewCowle/andrewcowle.github.io/master/slack.css',
   success: function(css) {
     $("<style></style>").appendTo('head').html(css);
   }
 });
});
