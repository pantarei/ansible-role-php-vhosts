Ansible Role for PHP FPM VirtualHost
====================================

[![Build Status](https://travis-ci.org/pantarei/ansible-role-php-fpm-vhosts.svg?branch=master)](https://travis-ci.org/pantarei/ansible-role-php-fpm-vhosts)
 [![GitHub tag](https://img.shields.io/github/tag/pantarei/ansible-role-php-fpm-vhosts.svg)](https://github.com/pantarei/ansible-role-php-fpm-vhosts)
 [![GitHub license](https://img.shields.io/github/license/pantarei/ansible-role-php-fpm-vhosts.svg)](https://github.com/pantarei/ansible-role-php-fpm-vhosts/blob/master/LICENSE)
 [![Ansible Role](https://img.shields.io/ansible/role/6382.svg)](https://galaxy.ansible.com/detail#/role/6382)

Ansible Role for PHP FPM VirtualHost Management.

Requirements
------------

This role require Ansible 1.9 or higher.

This role was designed for Ubuntu Server 14.04 LTS.

Role Variables
--------------

<table>
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">parameter</th>
<th align="left">required</th>
<th align="left">default</th>
<th align="left">choices</th>
<th align="left">comments</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left">php_fpm_vhosts_user</td>
<td align="left">yes</td>
<td align="left">example</td>
<td align="left"></td>
<td align="left">Username for virtual host user.</td>
</tr>
<tr class="even">
<td align="left">php_fpm_vhosts_pass</td>
<td align="left">yes</td>
<td align="left">uquaeZ6o</td>
<td align="left"></td>
<td align="left">Password for virtual host user.</td>
</tr>
<tr class="odd">
<td align="left">php_fpm_vhosts_home</td>
<td align="left">yes</td>
<td align="left">/home/example</td>
<td align="left"></td>
<td align="left">Location for the virtual host user home directory.</td>
</tr>
<tr class="even">
<td align="left">php_fpm_vhostsshort_open_tag</td>
<td align="left">yes</td>
<td align="left">Off</td>
<td align="left"></td>
<td align="left">Tells PHP whether the short form (&lt;? ?&gt;) of PHP's open tag should be allowed.</td>
</tr>
<tr class="odd">
<td align="left">php_fpm_vhostsmax_execution_time</td>
<td align="left">yes</td>
<td align="left">30</td>
<td align="left"></td>
<td align="left">This sets the maximum time in seconds a script is allowed to run before it is terminated by the parser.</td>
</tr>
<tr class="even">
<td align="left">php_fpm_vhostsmax_input_time</td>
<td align="left">yes</td>
<td align="left">60</td>
<td align="left"></td>
<td align="left">This sets the maximum time in seconds a script is allowed to parse input data, like POST and GET.</td>
</tr>
<tr class="odd">
<td align="left">php_fpm_vhostsmemory_limit</td>
<td align="left">yes</td>
<td align="left">256M</td>
<td align="left"></td>
<td align="left">This sets the maximum amount of memory in bytes that a script is allowed to allocate.</td>
</tr>
<tr class="even">
<td align="left">php_fpm_vhostserror_reporting</td>
<td align="left">yes</td>
<td align="left">E_ALL &amp; ~E_DEPRECATED &amp; ~E_STRICT</td>
<td align="left"></td>
<td align="left">Set the error reporting level.</td>
</tr>
<tr class="odd">
<td align="left">php_fpm_vhostsdisplay_errors</td>
<td align="left">yes</td>
<td align="left">Off</td>
<td align="left"></td>
<td align="left">This determines whether errors should be printed to the screen as part of the output or if they should be hidden from the user.</td>
</tr>
<tr class="even">
<td align="left">php_fpm_vhostsdisplay_startup_errors</td>
<td align="left">yes</td>
<td align="left">Off</td>
<td align="left"></td>
<td align="left">Even when display_errors is on, errors that occur during PHP's startup sequence are not displayed.</td>
</tr>
<tr class="odd">
<td align="left">php_fpm_vhostslog_errors</td>
<td align="left">yes</td>
<td align="left">On</td>
<td align="left"></td>
<td align="left">Tells whether script error messages should be logged to the server's error log or error_log.</td>
</tr>
<tr class="even">
<td align="left">php_fpm_vhostsignore_repeated_errors</td>
<td align="left">yes</td>
<td align="left">Off</td>
<td align="left"></td>
<td align="left">Do not log repeated messages.</td>
</tr>
<tr class="odd">
<td align="left">php_fpm_vhostsignore_repeated_source</td>
<td align="left">yes</td>
<td align="left">Off</td>
<td align="left"></td>
<td align="left">Ignore source of message when ignoring repeated messages.</td>
</tr>
<tr class="even">
<td align="left">php_fpm_vhostsreport_memleaks</td>
<td align="left">yes</td>
<td align="left">On</td>
<td align="left"></td>
<td align="left">If this parameter is set to On (the default), this parameter will show a report of memory leaks detected by the Zend memory manager.</td>
</tr>
<tr class="odd">
<td align="left">php_fpm_vhoststrack_errors</td>
<td align="left">yes</td>
<td align="left">Off</td>
<td align="left"></td>
<td align="left">If enabled, the last error message will always be present in the variable $php_errormsg.</td>
</tr>
<tr class="even">
<td align="left">php_fpm_vhostshtml_errors</td>
<td align="left">yes</td>
<td align="left">On</td>
<td align="left"></td>
<td align="left">Turn off HTML tags in error messages.</td>
</tr>
<tr class="odd">
<td align="left">php_fpm_vhostspost_max_size</td>
<td align="left">yes</td>
<td align="left">32M</td>
<td align="left"></td>
<td align="left">Sets max size of post data allowed.</td>
</tr>
<tr class="even">
<td align="left">php_fpm_vhosts_upload_tmp_dir</td>
<td align="left">yes</td>
<td align="left">/tmp</td>
<td align="left"></td>
<td align="left">The temporary directory used for storing files when doing file upload.</td>
</tr>
<tr class="odd">
<td align="left">php_fpm_vhostsupload_max_filesize</td>
<td align="left">yes</td>
<td align="left">32M</td>
<td align="left"></td>
<td align="left">The maximum size of an uploaded file.</td>
</tr>
<tr class="even">
<td align="left">php_fpm_vhostsdate_timezone</td>
<td align="left">yes</td>
<td align="left">Etc/UTC</td>
<td align="left"></td>
<td align="left">The default timezone used by all date/time functions.</td>
</tr>
<tr class="odd">
<td align="left">php_fpm_vhosts_session_save_path</td>
<td align="left">yes</td>
<td align="left">/tmp</td>
<td align="left"></td>
<td align="left">Defines the argument which is passed to the save handler.</td>
</tr>
</tbody>
</table>

Dependencies
------------

-   [hswong3i.php\_fpm](https://github.com/pantarei/ansible-role-php-fpm)

Example Playbook
----------------

    - hosts: servers
      roles:
        - { role: hswong3i.php_fpm_vhosts }

License
-------

-   Code released under [MIT](https://github.com/pantarei/ansible-role-php-fpm-vhosts/blob/master/LICENSE)
-   Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

Author Information
------------------

-   Wong Hoi Sing Edison
    -   <https://twitter.com/hswong3i>
    -   <https://github.com/hswong3i>

