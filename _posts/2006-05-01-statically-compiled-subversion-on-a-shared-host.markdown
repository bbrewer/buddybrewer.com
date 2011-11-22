--- 
layout: post
title: Statically compiled subversion on a shared host
---

Ever log into a shell account as a non-root user and find it lacking a
subversion client?  I ran into this recently while setting up <a
title="Capistrano deploy tool"
href="http://manuals.rubyonrails.com/read/book/17">capistrano</a> on my current
<a title="BlueHost.com" href="http://www.bluehost.com">hosting provider</a>. I
found the config options I wanted scattered across a few different web pages,
so for posterity here are the steps I followed to get a statically compiled
subversion client on my path:

<ol>
  <li>fetch the latest subversion tarball from <a class="ext-link"
  href="http://subversion.tigris.org/"><span
  class="icon">http://subversion.tigris.org</span></a></li>
  <li><code>./configure --enable-all-static --with-ssl --with-zlib</code></li>
	<li><code>make</code></li>
	<li><code>cp subversion/clients/cmdline/svn ~/bin/svn</code> (mkdir ~/bin if needed)</li>
	<li>add ~/bin to your $PATH</li>
</ol>

You can tune the options to ./configure as neccessary, but my goals were to get
an svn binary that would work against a subversion repository fronted by
Apache, accessed via HTTPS, with support for compression.
