`configure' configures this package to adapt to many kinds of systems.

Usage: ./configure [OPTION]... [VAR=VALUE]...

To assign environment variables (e.g., CC, CFLAGS...), specify them as
VAR=VALUE.  See below for descriptions of some of the useful variables.

Defaults for the options are specified in brackets.

Configuration:
  -h, --help              display this help and exit
      --help=short        display options specific to this package
      --help=recursive    display the short help of all the included packages
  -V, --version           display version information and exit
  -q, --quiet, --silent   do not print `checking ...' messages
      --cache-file=FILE   cache test results in FILE [disabled]
  -C, --config-cache      alias for `--cache-file=config.cache'
  -n, --no-create         do not create output files
      --srcdir=DIR        find the sources in DIR [configure dir or `..']

Installation directories:
  --prefix=PREFIX         install architecture-independent files in PREFIX
                          [/usr/local/apache2]
  --exec-prefix=EPREFIX   install architecture-dependent files in EPREFIX
                          [PREFIX]

By default, `make install' will install all the files in
`/usr/local/apache2/bin', `/usr/local/apache2/lib' etc.  You can specify
an installation prefix other than `/usr/local/apache2' using `--prefix',
for instance `--prefix=$HOME'.

For better control, use the options below.

Fine tuning of the installation directories:
  --bindir=DIR            user executables [EPREFIX/bin]
  --sbindir=DIR           system admin executables [EPREFIX/sbin]
  --libexecdir=DIR        program executables [EPREFIX/libexec]
  --sysconfdir=DIR        read-only single-machine data [PREFIX/etc]
  --sharedstatedir=DIR    modifiable architecture-independent data [PREFIX/com]
  --localstatedir=DIR     modifiable single-machine data [PREFIX/var]
  --runstatedir=DIR       modifiable per-process data [LOCALSTATEDIR/run]
  --libdir=DIR            object code libraries [EPREFIX/lib]
  --includedir=DIR        C header files [PREFIX/include]
  --oldincludedir=DIR     C header files for non-gcc [/usr/include]
  --datarootdir=DIR       read-only arch.-independent data root [PREFIX/share]
  --datadir=DIR           read-only architecture-independent data [DATAROOTDIR]
  --infodir=DIR           info documentation [DATAROOTDIR/info]
  --localedir=DIR         locale-dependent data [DATAROOTDIR/locale]
  --mandir=DIR            man documentation [DATAROOTDIR/man]
  --docdir=DIR            documentation root [DATAROOTDIR/doc/PACKAGE]
  --htmldir=DIR           html documentation [DOCDIR]
  --dvidir=DIR            dvi documentation [DOCDIR]
  --pdfdir=DIR            pdf documentation [DOCDIR]
  --psdir=DIR             ps documentation [DOCDIR]

System types:
  --build=BUILD     configure for building on BUILD [guessed]
  --host=HOST       cross-compile to build programs to run on HOST [BUILD]
  --target=TARGET   configure for building compilers for TARGET [HOST]

Optional Features:
  --disable-option-checking  ignore unrecognized --enable/--with options
  --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
  --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
  --enable-layout=LAYOUT
  --enable-dtrace         Enable DTrace probes
  --enable-hook-probes    Enable APR hook probes
  --enable-exception-hook Enable fatal exception hook
  --enable-load-all-modules
                          Load all modules
  --enable-maintainer-mode
                          Turn on debugging and compile time warnings and load
                          all compiled modules
  --enable-debugger-mode  Turn on debugging and compile time warnings and turn
                          off optimization
  --enable-pie            Build httpd as a Position Independent Executable
  --enable-modules=MODULE-LIST
                          Space-separated list of modules to enable | "all" |
                          "most" | "few" | "none" | "reallyall"
  --enable-mods-shared=MODULE-LIST
                          Space-separated list of shared modules to enable |
                          "all" | "most" | "few" | "reallyall"
  --enable-mods-static=MODULE-LIST
                          Space-separated list of static modules to enable |
                          "all" | "most" | "few" | "reallyall"
  --disable-authn-file    file-based authentication control
  --enable-authn-dbm      DBM-based authentication control
  --enable-authn-anon     anonymous user authentication control
  --enable-authn-dbd      SQL-based authentication control
  --enable-authn-socache  Cached authentication control
  --disable-authn-core    core authentication module
  --disable-authz-host    host-based authorization control
  --disable-authz-groupfile
                          'require group' authorization control
  --disable-authz-user    'require user' authorization control
  --enable-authz-dbm      DBM-based authorization control
  --enable-authz-owner    'require file-owner' authorization control
  --enable-authz-dbd      SQL based authorization and Login/Session support
  --disable-authz-core    core authorization provider vector module
  --enable-authnz-ldap    LDAP based authentication
  --enable-authnz-fcgi    FastCGI authorizer-based authentication and
                          authorization
  --disable-access-compat mod_access compatibility
  --disable-auth-basic    basic authentication
  --enable-auth-form      form authentication
  --enable-auth-digest    RFC2617 Digest authentication
  --enable-allowmethods   restrict allowed HTTP methods
  --enable-isapi          isapi extension support
  --enable-file-cache     File cache
  --enable-cache          dynamic file caching. At least one storage
                          management module (e.g. mod_cache_disk) is also
                          necessary.
  --enable-cache-disk     disk caching module
  --enable-cache-socache  shared object caching module
  --enable-socache-shmcb  shmcb small object cache provider
  --enable-socache-dbm    dbm small object cache provider
  --enable-socache-memcache
                          memcache small object cache provider
  --enable-socache-redis  redis small object cache provider
  --enable-socache-dc     distcache small object cache provider
  --enable-so             DSO capability. This module will be automatically
                          enabled unless you build all modules statically.
  --enable-watchdog       Watchdog module
  --enable-macro          Define and use macros in configuration files
  --enable-dbd            Apache DBD Framework
  --enable-bucketeer      buckets manipulation filter. Useful only for
                          developers and testing purposes.
  --enable-dumpio         I/O dump filter
  --enable-echo           ECHO server
  --enable-example-hooks  Example hook callback handler module
  --enable-case-filter    Example uppercase conversion filter
  --enable-case-filter-in Example uppercase conversion input filter
  --enable-example-ipc    Example of shared memory and mutex usage
  --enable-buffer         Filter Buffering
  --enable-data           RFC2397 data encoder
  --enable-ratelimit      Output Bandwidth Limiting
  --disable-reqtimeout    Limit time waiting for request from client
  --enable-ext-filter     external filter module
  --enable-request        Request Body Filtering
  --enable-include        Server Side Includes
  --disable-filter        Smart Filtering
  --enable-reflector      Reflect request through the output filter stack
  --enable-substitute     response content rewrite-like filtering
  --enable-sed            filter request and/or response bodies through sed
  --disable-charset-lite  character set translation. Enabled by default only
                          on EBCDIC systems.
  --enable-charset-lite   character set translation. Enabled by default only
                          on EBCDIC systems.
  --enable-deflate        Deflate transfer encoding support
  --enable-xml2enc        i18n support for markup filters
  --enable-proxy-html     Fix HTML Links in a Reverse Proxy
  --enable-brotli         Brotli compression support
  --enable-http           HTTP protocol handling. The http module is a basic
                          one that enables the server to function as an HTTP
                          server. It is only useful to disable it if you want
                          to use another protocol module instead. Don't
                          disable this module unless you are really sure what
                          you are doing. Note: This module will always be
                          linked statically.
  --disable-mime          mapping of file-extension to MIME. Disabling this
                          module is normally not recommended.
  --enable-ldap           LDAP caching and connection pooling services
  --disable-log-config    logging configuration. You won't be able to log
                          requests to the server without this module.
  --enable-log-debug      configurable debug logging
  --enable-log-forensic   forensic logging
  --enable-logio          input and output logging
  --enable-lua            Apache Lua Framework
  --enable-luajit         Enable LuaJit Support
  --disable-env           clearing/setting of ENV vars
  --enable-mime-magic     automagically determining MIME type
  --enable-cern-meta      CERN-type meta files
  --enable-expires        Expires header control
  --disable-headers       HTTP header control
  --enable-ident          RFC 1413 identity check
  --enable-usertrack      user-session tracking
  --enable-unique-id      per-request unique ids
  --disable-setenvif      basing ENV vars on headers
  --disable-version       determining httpd version in config files
  --enable-remoteip       translate header contents to an apparent client
                          remote_ip
  --enable-proxy          Apache proxy module
  --enable-proxy-connect  Apache proxy CONNECT module. Requires
                          --enable-proxy.
  --enable-proxy-ftp      Apache proxy FTP module. Requires --enable-proxy.
  --enable-proxy-http     Apache proxy HTTP module. Requires --enable-proxy.
  --enable-proxy-fcgi     Apache proxy FastCGI module. Requires
                          --enable-proxy.
  --enable-proxy-scgi     Apache proxy SCGI module. Requires --enable-proxy.
  --enable-proxy-uwsgi    Apache proxy UWSGI module. Requires --enable-proxy.
  --enable-proxy-fdpass   Apache proxy to Unix Daemon Socket module. Requires
                          --enable-proxy.
  --enable-proxy-wstunnel Apache proxy Websocket Tunnel module. Requires
                          --enable-proxy.
  --enable-proxy-ajp      Apache proxy AJP module. Requires --enable-proxy.
  --enable-proxy-balancer Apache proxy BALANCER module. Requires
                          --enable-proxy.
  --enable-proxy-express  mass reverse-proxy module. Requires --enable-proxy.
  --enable-proxy-hcheck   reverse-proxy health-check module. Requires
                          --enable-proxy and --enable-watchdog.
  --enable-session        session module
  --enable-session-cookie session cookie module
  --enable-session-crypto session crypto module
  --enable-session-dbd    session dbd module
  --enable-slotmem-shm    slotmem provider that uses shared memory
  --enable-slotmem-plain  slotmem provider that uses plain memory
  --enable-ssl            SSL/TLS support (mod_ssl)
  --enable-ssl-staticlib-deps
                          link mod_ssl with dependencies of OpenSSL's static
                          libraries (as indicated by "pkg-config --static").
                          Must be specified in addition to --enable-ssl.
  --enable-optional-hook-export
                          example optional hook exporter
  --enable-optional-hook-import
                          example optional hook importer
  --enable-optional-fn-import
                          example optional function importer
  --enable-optional-fn-export
                          example optional function exporter
  --enable-dialup         rate limits static files to dialup modem speeds
  --enable-static-support Build a statically linked version of the support
                          binaries
  --enable-static-htpasswd
                          Build a statically linked version of htpasswd
  --enable-static-htdigest
                          Build a statically linked version of htdigest
  --enable-static-rotatelogs
                          Build a statically linked version of rotatelogs
  --enable-static-logresolve
                          Build a statically linked version of logresolve
  --enable-static-htdbm   Build a statically linked version of htdbm
  --enable-static-ab      Build a statically linked version of ab
  --enable-static-checkgid
                          Build a statically linked version of checkgid
  --enable-static-htcacheclean
                          Build a statically linked version of htcacheclean
  --enable-static-httxt2dbm
                          Build a statically linked version of httxt2dbm
  --enable-static-fcgistarter
                          Build a statically linked version of fcgistarter
  --enable-http2          HTTP/2 protocol handling in addition to HTTP
                          protocol handling. Implemented by mod_http2. This
                          module requires a libnghttp2 installation. See
                          --with-nghttp2 on how to manage non-standard
                          locations. This module is usually linked shared and
                          requires loading.
  --enable-nghttp2-staticlib-deps
                          link mod_http2 with dependencies of libnghttp2's
                          static libraries (as indicated by "pkg-config
                          --static"). Must be specified in addition to
                          --enable-http2.
  --enable-proxy-http2    HTTP/2 proxy module. This module requires a
                          libnghttp2 installation. See --with-nghttp2 on how
                          to manage non-standard locations. Also requires
                          --enable-proxy.
  --enable-md             Managed Domain handling
  --enable-jansson-staticlib-deps
                          link mod_md with dependencies of libjansson's static
                          libraries (as indicated by "pkg-config --static").
                          Must be specified in addition to --enable-md.
  --enable-curl-staticlib-deps
                          link mod_md with dependencies of libcurl's static
                          libraries (as indicated by "pkg-config --static").
                          Must be specified in addition to --enable-md.
  --enable-lbmethod-byrequests
                          Apache proxy Load balancing by request counting
  --enable-lbmethod-bytraffic
                          Apache proxy Load balancing by traffic counting
  --enable-lbmethod-bybusyness
                          Apache proxy Load balancing by busyness
  --enable-lbmethod-heartbeat
                          Apache proxy Load balancing from Heartbeats
  --enable-tls            TLS protocol handling using rustls. Implemented by
                          mod_tls. This module requires a librustls
                          installation. See --with-rustls on how to manage
                          non-standard locations. This module is usually
                          linked shared and requires loading.
  --enable-mpms-shared=MPM-LIST
                          Space-separated list of MPM modules to enable for
                          dynamic loading. MPM-LIST=list | "all"
  --enable-unixd          unix specific support
  --enable-privileges     Per-virtualhost Unix UserIDs and enhanced security
                          for Solaris
  --enable-systemd        Systemd support
  --enable-heartbeat      Generates Heartbeats
  --enable-heartmonitor   Collects Heartbeats
  --enable-dav            WebDAV protocol handling. --enable-dav also enables
                          mod_dav_fs
  --disable-status        process/thread monitoring
  --disable-autoindex     directory listing
  --enable-asis           as-is filetypes
  --enable-info           server information
  --enable-suexec         set uid and gid for spawned processes
  --enable-cgid           CGI scripts. Enabled by default with threaded MPMs
  --enable-cgi            CGI scripts. Enabled by default with non-threaded
                          MPMs
  --enable-dav-fs         DAV provider for the filesystem. --enable-dav also
                          enables mod_dav_fs.
  --enable-dav-lock       DAV provider for generic locking
  --enable-vhost-alias    mass virtual hosting module
  --enable-negotiation    content negotiation
  --disable-dir           directory request handling
  --enable-imagemap       server-side imagemaps
  --enable-actions        Action triggering on requests
  --enable-speling        correct common URL misspellings
  --enable-userdir        mapping of requests to user-specific directories
  --disable-alias         mapping of requests to different filesystem parts
  --enable-rewrite        rule based URL manipulation
  --enable-suexec-capabilities
                          Use Linux capability bits not setuid root suexec
  --enable-v4-mapped      Allow IPv6 sockets to handle IPv4 connections

Optional Packages:
  --with-PACKAGE[=ARG]    use PACKAGE [ARG=yes]
  --without-PACKAGE       do not use PACKAGE (same as --with-PACKAGE=no)
  --with-included-apr     Use bundled copies of APR/APR-Util
  --with-apr=PATH         prefix for installed APR or the full path to
                             apr-config
  --with-apr-util=PATH    prefix for installed APU or the full path to
                             apu-config
  --with-pcre=PATH        Use external PCRE library
  --with-port=PORT        Port on which to listen (default is 80)
  --with-sslport=SSLPORT  Port on which to securelisten (default is 443)
  --with-distcache=PATH   Distcache installation directory
  --with-z=PATH           use a specific zlib library
  --with-libxml2=PATH     location for libxml2
  --with-brotli=PATH      Brotli installation directory
  --with-lua=PATH         Path to the Lua installation prefix
  --with-ssl=PATH         OpenSSL installation directory
  --with-nghttp2=PATH     nghttp2 installation directory
  --with-jansson=PATH     jansson installation directory
  --with-curl=PATH        curl installation directory
  --with-rustls=PATH      rustls installation directory
  --with-mpm=MPM          Choose the process model for Apache to use by
                          default. MPM={event|worker|prefork|winnt} This will
                          be statically linked as the only available MPM
                          unless --enable-mpms-shared is also specified.
  --with-module=module-type:module-file
                          Enable module-file in the modules/<module-type>
                          directory.
  --with-program-name     alternate executable name
  --with-suexec-bin       Path to suexec binary
  --with-suexec-caller    User allowed to call SuExec
  --with-suexec-userdir   User subdirectory
  --with-suexec-docroot   SuExec root directory
  --with-suexec-uidmin    Minimal allowed UID
  --with-suexec-gidmin    Minimal allowed GID
  --with-suexec-logfile   Set the logfile
  --with-suexec-syslog    Use syslog for suexec logging
  --with-suexec-safepath  Set the safepath
  --with-suexec-umask     umask for suexec'd process

Some influential environment variables:
  CC          C compiler command
  CFLAGS      C compiler flags
  LDFLAGS     linker flags, e.g. -L<lib dir> if you have libraries in a
              nonstandard directory <lib dir>
  LIBS        libraries to pass to the linker, e.g. -l<library>
  CPPFLAGS    (Objective) C/C++ preprocessor flags, e.g. -I<include dir> if
              you have headers in a nonstandard directory <include dir>
  CPP         C preprocessor

Use these variables to override the choices made by `configure' or to help
it to find libraries and programs with nonstandard names/locations.

Report bugs to the package provider.
