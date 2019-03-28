<!DOCTYPE html>
<html lang="en-US">
  <head>
    <meta charset='utf-8'>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <link rel="stylesheet" href="/digits/assets/css/style.css?v=f8d0d60de6fb0dbbd6b05bec420b55c1d9bc462b">
    <link rel="stylesheet" type="text/css" href="/digits/assets/css/print.css" media="print">
    <!--[if lt IE 9]>
    <script src="//html5shiv.googlecode.com/svn/trunk/html5.js"></script>
    <![endif]-->

<!-- Begin Jekyll SEO tag v2.5.0 -->
<title>digits</title>
<meta name="generator" content="Jekyll v3.7.4" />
<meta property="og:title" content="digits" />
<meta property="og:locale" content="en_US" />
<link rel="canonical" href="https://ics-software-engineering.github.io/digits/" />
<meta property="og:url" content="https://ics-software-engineering.github.io/digits/" />
<meta property="og:site_name" content="digits" />
<script type="application/ld+json">
{"@type":"WebSite","url":"https://ics-software-engineering.github.io/digits/","name":"digits","headline":"digits","@context":"http://schema.org"}</script>
<!-- End Jekyll SEO tag -->

  </head>

  <body>
    <div id="container">
      <div class="inner">

        <header>
          <h1>digits</h1>
          <h2></h2>
        </header>
        <section id="downloads" class="clearfix">
          
	
        </section>
        <hr>
        <section id="main_content">
          <p><img src="doc/landing.png" /></p>

<p>Digits is an application that will</p>

<ul>
  <li>Allow you to create an account.</li>
  <li>Create contacts.</li>
  <li>Create notes for your contacts.</li>
</ul>

<h3>Installation</h3>

<p>Install Meteor <a href="https://www.meteor.com/install">here</a>.</p>

<p>Then, <a href="https://github.com/peter-newton/digits">download a copy of Digits</a>. Note that Digits is a private repo and so you will need to request permission from the author to gain access to the repo.</p>

<p>Once that is finished, open your command prompt and cd into the app directory and install the required libraries with:</p>

<code>$ meteor npm install
</code>

<p>When the libraries are installed, run the application in the command prompt with this.</p>
<code>$ meteor npm run start
</code>

<p>While the program is running, you will see a stream of infomation that will look like similar to this.</p>

<code>meteor npm run start

> meteor-application-template-react@ start C:\Users\peace\Documents\github\PeterNewton\digits\app
> meteor --no-release-check --settings ../config/settings.development.json

[[[[[ C:\Users\peace\Documents\github\PeterNewton\digits\app ]]]]]

=> Started proxy.
=> Started MongoDB.
W20190327-20:16:14.366(-10)? (STDERR) Note: you are using a pure-JavaScript implementation of bcrypt.
W20190327-20:16:14.614(-10)? (STDERR) While this implementation will work correctly, it is known to be
W20190327-20:16:14.615(-10)? (STDERR) approximately three times slower than the native implementation.
W20190327-20:16:14.617(-10)? (STDERR) In order to use the native implementation instead, run
W20190327-20:16:14.618(-10)? (STDERR)
W20190327-20:16:14.619(-10)? (STDERR)   meteor npm install --save bcrypt
W20190327-20:16:14.619(-10)? (STDERR)
W20190327-20:16:14.620(-10)? (STDERR) in the root directory of your application.
=> Started your app.

=> App running at: http://localhost:3000/
   Type Control-C twice to stop.
</code>

<p>Note regarding bcrypt warning. You will also get the following message when you run this application:</p>

<code>Note: you are using a pure-JavaScript implementation of bcrypt.
While this implementation will work correctly, it is known to be
approximately three times slower than the native implementation.
In order to use the native implementation instead, run

  meteor npm install --save bcrypt

in the root directory of your application.
</code>

<p>On some operating systems (particularly Windows), installing bcrypt is much more difficult than implied by the above message. Bcrypt is only used in Meteor for password checking, so the performance implications are negligible until your site has very high traffic. You can safely ignore this warning without any problems during initial stages of development.</p>

<p>When the application is running without errors, open a web browser and type in this web address: <a href="http://localhost:3000">http://localhost:3000</a>.  You can login using the default accounts "john@foo.com" or the admin account "admin@foo.com".  Both accounts will have a default password of "changeme".  If you don't want to use the default information then register a new account.</p>

<h2>User Interface Walkthrough</h2>

<h4>Landing Page</h4>

<p>This is the page that you will first encounter when opening up the application.  It contains information on the capabilities that this application can do.</p>

<p><img src="doc/landing.png" /></p>

<h4>Register</h4>

<p>If you don't want to use the default information, then you can register by clicking on “Login”, and then “Sign Up”:</p>

<p><img src="doc/register.png" /></p>

<h4>Sign in</h4>

<p>In order to sign in, you must click on "Login" and then click on "Signin".  This will take you to the "Sign In" page for you to input your credentials to log into the application.</p>

<p><img src="doc/signin.png" /></p>

<h4>User home page</h4>

<p>Once you have signed in, you will see your home page. Your home page can be verified by observing the NavBar which contains links to "list contact" and "add new contacts"</p>

<p><img src="doc/home.png" /></p>

<h4>List Contacts</h4>

<p>This link will direct you to a page that has all of the users contacts that were saved.  As part of the contact listings, each contact card will have the ability to edit information or leave a timestamped note.</p>

<p><img src="doc/list-contacts.png" /></p>

<h4>Edit Contacts</h4>

<p>By selecting "Edit" on the contact card, you will be brought to the "Edit Contacts" page which will have informational fields where you can update the information for each contact.</p>

<p><img src="doc/edit-contact.png" /></p>

<h4>Admin mode</h4>

<p>You can give users administrative rights within the settings file.  Once designated as an "Admin", an additional "Admin" link will become available on the NavBar which will open a page that lists all contact from every user.</p>

<p><img src="doc/admin-page.png" /></p>   
  </body>
</html>
