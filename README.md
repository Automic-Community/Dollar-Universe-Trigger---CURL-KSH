*Dollar Universe Trigger - CURL KSH *
=============


This script is an example of how to use Dollar Universe Triggers with the curl utility.
http://github.com/Automic-Community/Dollar-Universe-Trigger---CURL-KSH-

<!-- List of attached files -->
Contents of Solution Package:

						
								*Dollar_Universe-Trigger_Curl.zip
								
						


Documenation and Instructions
---

<div class="ipsType_textblock ipsPad_half description_content"><strong class="bbc"><span><span>Description</span></span></strong><br />This script is an example of how to use Dollar Universe Triggers with the curl utility.<br />Besides curl, this script uses sed, tr and awk.<br /><br /><strong class="bbc"><span>Operating systems</span></strong><br />Linux.<br />This script may run on Unix plateforms, but please note that, due to the variety of implementations, some adjustments may be needed.<br />For example, on SunOS, you may have to change awk by nawk.<br /><br />This script has been briefly tested on:
<ul class="bbc">
<li>Linux 2.6.32-431.el6.x86_64 x86_64 GNU/Linux , curl 7.19.7</li>
<li>Linux 2.6.18-238.9.1.el5PAE i386 GNU/Linux, curl 7.15.5</li>
<li>SunOS 5.11 11.0 sun4u sparc SUNW,SPARC-Enterprise, curl 7.21.2, (need to replace awk by nawk)</li>
</ul>
<span><strong class="bbc">Prerequisites</strong></span>
<ul class="bbc">
<li>Having curl utility installed (version 7.18.0 minimum is required to use --data-urlencode). See <a class="bbc_url" title="External link" href="http://curl.haxx.se" rel="nofollow external">http://curl.haxx.se</a></li>
</ul>
<strong class="bbc"><span><span>How to use</span></span></strong>
<ul class="bbc">
<li>Replace the variables defined at the beginning of the script</li>
<li>HOST: the hostname of the targeted Dollar Universe node</li>
<li>PORT: the port number of the Dollar Universe API</li>
<li>USER: the login used for authentication</li>
<li>PWD: the password used for authentication</li>
<li>EVENT: the name of the event type to send</li>
<li>AREA: the Dollar Universe targeted area</li>
</ul>
<ul class="bbc">
<li>Run the script</li>
</ul>
<strong class="bbc">Note</strong>: If the curl version is greater than 7.18.0, the data are sent in the application/x-www-form-urlencoded format; otherwise, the data are sent in text/plain format (--data-urlencode unsupported).<br /><br /><br /><span><strong class="bbc">Output</strong></span><br />The output gives information about the three steps of the script:
<ul class="bbc">
<li>Login</li>
<li>Event type send</li>
<li>Logout</li>
</ul>
<pre class="prettyprint lang-auto linenums:0 prettyprinted"><span class="typ">Script</span><span class="pln"> launched at </span><span class="pun">&lt;</span><span class="pln">date </span><span class="kwd">and</span><span class="pln"> time</span><span class="pun">&gt;</span><span class="pln">
</span><span class="typ">Login</span><span class="pln"> on </span><span class="str">&lt;host&gt;</span><span class="pun">:&lt;</span><span class="pln">port</span><span class="pun">&gt;</span><span class="pln"> </span><span class="pun">--&gt;</span><span class="pln"> </span><span class="typ">Success</span><span class="pln"> token </span><span class="kwd">is</span><span class="pln"> </span><span class="str">&lt;token&gt;</span><span class="pln">

</span><span class="typ">Send</span><span class="pln"> </span><span class="kwd">event</span><span class="pln"> </span><span class="pun">&lt;</span><span class="kwd">event</span><span class="pln"> name</span><span class="pun">&gt;</span><span class="pln"> </span><span class="pun">--&gt;</span><span class="pln"> </span><span class="typ">Incomplete</span><span class="pln">
</span><span class="pun">=&gt;</span><span class="pln"> </span><span class="typ">Trigger</span><span class="pun">:</span><span class="pln"> DEMO TRIGGER </span><span class="pun">--&gt;</span><span class="pln"> </span><span class="typ">Launch</span><span class="pln"> number</span><span class="pun">:</span><span class="pln"> </span><span class="lit">0000995</span><span class="pln">
</span><span class="pun">=&gt;</span><span class="pln"> </span><span class="typ">Trigger</span><span class="pun">:</span><span class="pln"> DEMO TRIGGER </span><span class="lit">2</span><span class="pln"> </span><span class="pun">--&gt;</span><span class="pln"> </span><span class="typ">Launch</span><span class="pln"> number</span><span class="pun">:</span><span class="pln"> </span><span class="lit">0000996</span><span class="pln">
</span><span class="pun">=&gt;</span><span class="pln"> </span><span class="typ">Trigger</span><span class="pun">:</span><span class="pln"> INCOMPLETE</span><span class="pun">:</span><span class="pln"> </span><span class="pun">--&gt;</span><span class="pln"> </span><span class="typ">Error</span><span class="pln"> </span><span class="lit">702</span><span class="pun">:</span><span class="pln"> </span><span class="typ">No</span><span class="pln"> task associated </span><span class="kwd">with</span><span class="pln"> trigger</span><span class="pun">.</span><span class="pln">

</span><span class="typ">Logout</span><span class="pln"> </span><span class="pun">--&gt;</span><span class="pln"> </span><span class="typ">Success</span></pre>
</div>

Copyright and License
---

Solutions, Templates, Actions and other content available on the Automic Marketplace subject to the Automic [Developers Distribution License] (http://automic.com/developers-distribution-license) as well as the Automic Community [Terms of Service] (http://automic.com/community-terms-of-service).
Automic does not support, maintain or warrant any content submitted by the Automic Community.



Questions or Need Help? 
---
Any questions or comments? Converse with your fellow Users in the [Automic Community] (https://community.automic.com).