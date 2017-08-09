
------------------------------------------------------------------------------------------------------
APACHE HTTP SERVER - 

------------------------------------------------------------------------------------------------------

Ultima versão --

http://www.apache.org/dist/httpd/CHANGES_2.4.27

                                                         -*- coding: utf-8 -*-

Changes with Apache 2.4.27

  *) SECURITY: CVE-2017-9789 (cve.mitre.org)
     mod_http2: Read after free. When under stress, closing many connections,
     the HTTP/2 handling code would sometimes access memory after it has been
     freed, resulting in potentially erratic behaviour.
     [Stefan Eissing]

  *) SECURITY: CVE-2017-9788 (cve.mitre.org)
     mod_auth_digest: Uninitialized memory reflection.  The value placeholder
     in [Proxy-]Authorization headers type 'Digest' was not initialized or
     reset before or between successive key=value assignments.
     [William Rowe]

  *) COMPATIBILITY: mod_lua: Remove the undocumented exported 'apr_table'
     global variable when using Lua 5.2 or later. This was exported as a
     side effect from luaL_register, which is no longer supported as of
     Lua 5.2 which deprecates pollution of the global namespace.
     [Rainer Jung]

  *) COMPATIBILITY: mod_http2: Disable and give warning when using Prefork.
     The server will continue to run, but HTTP/2 will no longer be negotiated.
     [Stefan Eissing]

  *) COMPATIBILITY: mod_proxy_fcgi: Revert to 2.4.20 FCGI behavior for the
     default ProxyFCGIBackendType, fixing a regression with PHP-FPM. PR 61202.
     [Jacob Champion, Jim Jagielski]

  *) mod_lua: Improve compatibility with Lua 5.1, 5.2 and 5.3.
     PR58188, PR60831, PR61245. [Rainer Jung]
  
  *) mod_http2: Simplify ready queue, less memory and better performance. Update
     mod_http2 version to 1.10.7. [Stefan Eissing]
  
  *) Allow single-char field names inadvertently disallowed in 2.4.25.
     PR 61220. [Yann Ylavic]

  *) htpasswd / htdigest: Do not apply the strict permissions of the temporary
     passwd file to a possibly existing passwd file. PR 61240. [Ruediger Pluem]

  *) core: Avoid duplicate HEAD in Allow header.
     This is a regression in 2.4.24 (unreleased), 2.4.25 and 2.4.26.
     PR 61207. [Christophe Jaillet]



  [Apache 2.3.0-dev includes those bug fixes and changes with the
   Apache 2.2.xx tree as documented, and except as noted, below.]

Changes with Apache 2.2.x and later:

  *) http://svn.apache.org/viewvc/httpd/httpd/branches/2.2.x/CHANGES?view=markup

Changes with Apache 2.0.x and later:

  *) http://svn.apache.org/viewvc/httpd/httpd/branches/2.0.x/CHANGES?view=markup

Penultima Versão  - 

http://www.apache.org/dist/httpd/CHANGES_2.2.34

                                                         -*- coding: utf-8 -*-
Changes with Apache 2.2.34 (final)

  *) SECURITY: CVE-2017-9788 (cve.mitre.org)
     mod_auth_digest: Uninitialized memory reflection.  The value placeholder
     in [Proxy-]Authorization headers type 'Digest' was not initialized or
     reset before or between successive key=value assignments.
     [William Rowe]

  *) Allow single-char field names inadvertantly disallowed in 2.2.32.
     PR 61220. [Yann Ylavic]

Changes with Apache 2.2.33 (not released)

  *) SECURITY: CVE-2017-7668 (cve.mitre.org)
     The HTTP strict parsing changes added in 2.2.32 and 2.4.24 introduced a
     bug in token list parsing, which allows ap_find_token() to search past
     the end of its input string. By maliciously crafting a sequence of
     request headers, an attacker may be able to cause a segmentation fault,
     or to force ap_find_token() to return an incorrect value.
     [Jacob Champion]

  *) SECURITY: CVE-2017-3169 (cve.mitre.org)
     mod_ssl may dereference a NULL pointer when third-party modules call
     ap_hook_process_connection() during an HTTP request to an HTTPS port.
     [Yann Ylavic]

  *) SECURITY: CVE-2017-3167 (cve.mitre.org)
     Use of the ap_get_basic_auth_pw() by third-party modules outside of the
     authentication phase may lead to authentication requirements being
     bypassed.
     [Emmanuel Dreyfus <manu netbsd.org>, Jacob Champion, Eric Covener]

  *) SECURITY: CVE-2017-7679 (cve.mitre.org)
     mod_mime can read one byte past the end of a buffer when sending a
     malicious Content-Type response header.  [Yann Ylavic]
  
  *) Fix HttpProtocolOptions to inherit from global to VirtualHost scope.
     [Joe Orton]

------------------------------------------------------------------------------------------------------
nginx
------------------------------------------------------------------------------------------------------


2017-08-08	
nginx-1.13.4 mainline version has been released, featuring the mirror module.

2017-07-11	
nginx-1.12.1 stable and nginx-1.13.3 mainline versions have been released with a fix for the integer overflow in the range filter vulnerability (CVE-2017-7529).

2017-06-27	
nginx-1.13.2 mainline version has been released.

2017-05-30	
nginx-1.13.1 mainline version has been released.

2017-04-25	
nginx-1.13.0 mainline version has been released.

2017-04-12	
nginx-1.12.0 stable version has been released, incorporating new features and bug fixes from the 1.11.x mainline branch - including variables support and other improvements in the stream module, HTTP/2 fixes, support for multiple SSL certificates of different types, improved dynamic modules support, and more.

---------------------------------------------------------------------------------------------------------------
wordpress
---------------------------------------------------------------------------------------------------------------
Versão mais recente
4.8.1	02-08-2017	zip (md5)	tar.gz (md5)
Ramo 4.8
4.8.1	02-08-2017	zip (md5)	tar.gz (md5)
4.8	14-07-2017	zip (md5)	tar.gz (md5)
