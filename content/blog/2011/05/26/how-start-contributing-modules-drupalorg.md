---
title: "How to Start Contributing to Modules on Drupal.org"
date: 2011-05-26
tags: Drupal Dev Notes, drupal-planet, drupal-planet
---
<p>Drupal Dev Notes is a new series of screencasts that I'm starting to share all of the Drupal development know-how, habits and tricks that I wish I'd learned the easy way.</p>

<p>The first of these is how to contribute to projects on drupal.org. The best way to get started with contrib is by making small fixes to other people's projects. This way you can learn Drupal coding standards and best practices gradually, with help from other Drupal developers. It can also be really fun :)</p>
READMORE<p>UPDATE: I highly recommend reading <a href="http://www.lullabot.com/articles/how-solve-all-your-problems">How to Solve All Your Problems</a> first, especially if you haven't been active on the issue queue before.</p><object width="480" height="390"><param name="movie" value="http://www.youtube.com/v/hRlXTinjs4o?fs=1&amp;hl=en_US&amp;rel=0"></param><param name="allowFullScreen" value="true"></param><param name="allowscriptaccess" value="always"></param><embed src="http://www.youtube.com/v/hRlXTinjs4o?fs=1&amp;hl=en_US&amp;rel=0" type="application/x-shockwave-flash" width="480" height="390" allowscriptaccess="always" allowfullscreen="true"></embed></object><a href="http://youtu.be/hRlXTinjs4o">Link to video</a><ol><li><strong>Install Git</strong><br />There&#39;s <a href="http://drupal.org/node/1010894">installation instructions for Git</a> on drupal.org. If those don&#39;t work for you, try&nbsp;<a href="http://help.github.com">http://help.github.com/ </a>and then follow <a href="http://vimeo.com/20459209">Randy Fay&#39;s screencast </a>to hook it up to Drupal (or read the <a href="http://drupal.org/node/1013552">instructions on drupal.org</a>).</li><li><strong>Choose issue</strong><br />You can either look at issues on a specific project, or a great way to find easy ones is to <a href="http://drupal.org/project/issues/search?issue_tags=Novice">look for the Novice tag</a>. You want the&nbsp;<a href="http://drupal.org/node/156119">issue status</a>&nbsp;to be either &#39;active&#39; or &#39;needs work&#39;.</li><li><strong>Download project</strong><br />Each project has Git instructions. Choose the latest branch, which will probably be 7.x-?.x or master. Click &#39;Show&#39; and copy the command. Then run the command in the sites/all/modules directory.</li><li><strong>Find bug</strong><br /><code>egrep -r hook_node_info simpletest_example/</code></li><li><strong>Make branch</strong><br /><code>git checkout -b [short description]-[issue-number]</code></li><li><strong>Fix code</strong><br />Refer to <a href="http://drupal.org/coding-standards">coding standards</a> for code style.</li><li><strong>Create patch</strong><br /><code>git diff &gt; [description]-[issue-number]-[comment-number].patch</code><br />Randy Fay has a great post about <a href="http://randyfay.com/node/97">patching with Git</a>.</li><li><strong>Upload patch for review</strong><br />People often use <a href="http://drupal.org/project/dreditor">Dreditor</a>&nbsp;to review patches.</li><li><strong>Make revisions</strong><br />Once you get feedback, you can make revisions to the patch.<br />Refresh your repo using&nbsp;<br /><code>git checkout [version]<br />git pull</code><br />Then re-apply changes:<br /><code>git apply -v [patchname].patch</code></li></ol><h2>Other Links</h2><ul><li>Jacine gives an <a href="http://jacine.net/post/8419331209/patches">in depth guide</a> to how patches work</li><li>
<a href="http://drupal.org/node/1054616">Advanced patch contributor guide</a></li><li><a href="http://drupal.org/node/45111">Priority levels for an issue</a></li><li><a href="http://randyfay.com/node/97">Randy Fay&#39;s blog</a></li></ul>