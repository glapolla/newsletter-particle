# Newsletter-Particle
Newsletter Particle From Rockettheme modified for Mail Chimp

## Getting Started

## Installing

First thing you will need to do is copy the contents of the particles folder newsletter.html.twig and newsletter.yaml files to TEMPLATE_DIR/custom/particles. If the particles directory does not already exist in your custom folder, you will have to create it.

Next copy the _newsletter.scss from the scss folder to the TEMPLATE_DIR/custom/scss.  If the scss directory does not already exist in your custom folder, you will have to create it. If you do not have a custom.css file also copy the custom.scss file.  IF you have a custom.css add file @import "dependencies"; and @import "newsletter"; at the top of the file on seperate lines.
 
Go to https://kb.mailchimp.com/lists/signup-forms/host-your-own-signup-forms and follow the instructions there.  The part you will need is:````

```
<form action="http://mailchimp.us8.list-manage.com/subscribe/post" method="POST">

<input type="hidden" name="u" value="a123cd45678ef90g7h1j7k9lm">

<input type="hidden" name="id" value="ab2c468d10">
```

This info will be added in the particle config when you add the particle to your template.  on the url drop the http:// part when you enter it.  The u value is the user id and the id is the list id.  insert these into the appropriate locations in the particle config.

