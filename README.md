#getnmail - _get this nickname email_

A command line tool to list emails of a given nickname that was previously
registered using this same tool.

###License: GPL version 3 - no later version option.

###Frequently asked questions:
**Why no later version option for the license ?**

Currently version 3 is the latest version and I can't possibly agree with something
that I don't know/understand and most importantly doesn't exist. So any reference to later version is a no go at this point. If the current license is a trouble for you, feel free to contact me, maybe we can find something suitable for everyone.

**Why do I need a tool like this ?**
Nicknames are awesome, usually short and easy to remember, but emails, depends on a lot of factors.
I don't want to remember domains of my friends and I don't want to open my contact book for it.
<br>
**Why a command line tool though ?**
Because It's where I need it ? Think of authors on programming projects,
manual gpg signing and so on. It just gets painful.
<br/>

##documentation - guidelines + [todo]

**user:**
Register a nickname/user ( notice nicknames are case sensitive )
<pre>
getnmail --register "nickname" --email "address@domain.tld"
</pre>
<br/>
Register a nickname/user with multiple emails
<pre>
getnmail --register "nickname" --email "address@domain.tld" "address2@domain.tld" "address3@domain.tld"
</pre>
<br/>
Get the email of a given nickname 
<pre>
getnmail nickname
</pre>
<br/>
Get the email of a partially known the nickname
<br/>
for cases where you don't know the start
<pre>
getnmail *par
</pre>
<br/>
for cases where you don't know the end
<pre>
getnmail par*
</pre>
<br/>
for cases where you only know the middle
<pre>
getnmail *par*
</pre>
<br/>
get the nickname by email instead
<pre>
getnmail --get-nickname "address@domain.tld"
</pre>