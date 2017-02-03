# load balacing

https://www.youtube.com/watch?v=yNuuoQLw0tA#t=798.460003

https://www.youtube.com/watch?v=1Sdr42EMwEI

https://www.youtube.com/user/MaAbani/videos?sort=dd&shelf_id=1&view=0

https://www.youtube.com/watch?v=bNFCEMPf3h8

http://www.apachehaus.com/cgi-bin/download.plx

https://www.youtube.com/watch?v=kDZ5KkVQDxE

https://www.youtube.com/watch?v=V2L7_xAGhqM&feature=youtu.be

https://www.youtube.com/watch?v=Njx1V4ZW_g0

```code
...
apply plugin: 'war'

war {
    baseName = 'myapp'
    version =  '0.5.0'
}

repositories {
    jcenter()
    maven { url "http://repo.spring.io/libs-snapshot" }
}

dependencies {
    compile("org.springframework.boot:spring-boot-starter-web")
    providedRuntime("org.springframework.boot:spring-boot-starter-tomcat") //this is main point for library
    ...
}
```

https://www.mulesoft.com/tcat/apache-tomcat-mod-jk-connector-configuration

#configure in server.xml

##turn on module in apache24

```code
LoadModule access_compat_module modules/mod_access_compat.so

LoadModule actions_module modules/mod_actions.so

LoadModule alias_module modules/mod_alias.so

LoadModule allowmethods_module modules/mod_allowmethods.so

LoadModule asis_module modules/mod_asis.so

LoadModule auth_basic_module modules/mod_auth_basic.so

#LoadModule auth_digest_module modules/mod_auth_digest.so

#LoadModule auth_form_module modules/mod_auth_form.so

#LoadModule authn_anon_module modules/mod_authn_anon.so

LoadModule authn_core_module modules/mod_authn_core.so

#LoadModule authn_dbd_module modules/mod_authn_dbd.so

#LoadModule authn_dbm_module modules/mod_authn_dbm.so

LoadModule authn_file_module modules/mod_authn_file.so

#LoadModule authn_socache_module modules/mod_authn_socache.so

#LoadModule authnz_fcgi_module modules/mod_authnz_fcgi.so

#LoadModule authnz_ldap_module modules/mod_authnz_ldap.so

LoadModule authz_core_module modules/mod_authz_core.so

#LoadModule authz_dbd_module modules/mod_authz_dbd.so

#LoadModule authz_dbm_module modules/mod_authz_dbm.so

LoadModule authz_groupfile_module modules/mod_authz_groupfile.so

LoadModule authz_host_module modules/mod_authz_host.so

#LoadModule authz_owner_module modules/mod_authz_owner.so

LoadModule authz_user_module modules/mod_authz_user.so

LoadModule autoindex_module modules/mod_autoindex.so

#LoadModule buffer_module modules/mod_buffer.so

#LoadModule cache_module modules/mod_cache.so

#LoadModule cache_disk_module modules/mod_cache_disk.so```

#LoadModule cache_socache_module modules/mod_cache_socache.so

#LoadModule cern_meta_module modules/mod_cern_meta.so

LoadModule cgi_module modules/mod_cgi.so

#LoadModule charset_lite_module modules/mod_charset_lite.so

#LoadModule data_module modules/mod_data.so

#LoadModule dav_module modules/mod_dav.so

#LoadModule dav_fs_module modules/mod_dav_fs.so

#LoadModule dav_lock_module modules/mod_dav_lock.so

#LoadModule dbd_module modules/mod_dbd.so

#LoadModule deflate_module modules/mod_deflate.so

LoadModule dir_module modules/mod_dir.so

#LoadModule dumpio_module modules/mod_dumpio.so

LoadModule env_module modules/mod_env.so

#LoadModule expires_module modules/mod_expires.so

#LoadModule ext_filter_module modules/mod_ext_filter.so

#LoadModule file_cache_module modules/mod_file_cache.so

#LoadModule filter_module modules/mod_filter.so

#LoadModule headers_module modules/mod_headers.so

#LoadModule heartbeat_module modules/mod_heartbeat.so

#LoadModule heartmonitor_module modules/mod_heartmonitor.so

#LoadModule http2_module modules/mod_http2.so

#LoadModule ident_module modules/mod_ident.so

#LoadModule imagemap_module modules/mod_imagemap.so

LoadModule include_module modules/mod_include.so

LoadModule info_module modules/mod_info.so

LoadModule isapi_module modules/mod_isapi.so

#LoadModule lbmethod_bybusyness_module modules/mod_lbmethod_bybusyness.so

#LoadModule lbmethod_byrequests_module modules/mod_lbmethod_byrequests.so

#LoadModule lbmethod_bytraffic_module modules/mod_lbmethod_bytraffic.so

#LoadModule lbmethod_heartbeat_module modules/mod_lbmethod_heartbeat.so

#LoadModule ldap_module modules/mod_ldap.so

#LoadModule logio_module modules/mod_logio.so

LoadModule log_config_module modules/mod_log_config.so

#LoadModule log_debug_module modules/mod_log_debug.so

#LoadModule log_forensic_module modules/mod_log_forensic.so

#LoadModule lua_module modules/mod_lua.so

#LoadModule macro_module modules/mod_macro.so

LoadModule mime_module modules/mod_mime.so

#LoadModule mime_magic_module modules/mod_mime_magic.so

LoadModule negotiation_module modules/mod_negotiation.so

LoadModule proxy_module modules/mod_proxy.so

LoadModule proxy_ajp_module modules/mod_proxy_ajp.so

#LoadModule proxy_balancer_module modules/mod_proxy_balancer.so

#LoadModule proxy_connect_module modules/mod_proxy_connect.so

#LoadModule proxy_express_module modules/mod_proxy_express.so

#LoadModule proxy_fcgi_module modules/mod_proxy_fcgi.so

#LoadModule proxy_ftp_module modules/mod_proxy_ftp.so

#LoadModule proxy_html_module modules/mod_proxy_html.so

#LoadModule proxy_hcheck_module modules/mod_proxy_hcheck.so

#LoadModule proxy_http_module modules/mod_proxy_http.so

#LoadModule proxy_http2_module modules/mod_proxy_http2.so

#LoadModule proxy_scgi_module modules/mod_proxy_scgi.so

#LoadModule proxy_wstunnel_module modules/mod_proxy_wstunnel.so

#LoadModule ratelimit_module modules/mod_ratelimit.so

#LoadModule reflector_module modules/mod_reflector.so

#LoadModule remoteip_module modules/mod_remoteip.so

#LoadModule request_module modules/mod_request.so

#LoadModule reqtimeout_module modules/mod_reqtimeout.so

#LoadModule rewrite_module modules/mod_rewrite.so

#LoadModule sed_module modules/mod_sed.so

#LoadModule session_module modules/mod_session.so

#LoadModule session_cookie_module modules/mod_session_cookie.so

#LoadModule session_crypto_module modules/mod_session_crypto.so

#LoadModule session_dbd_module modules/mod_session_dbd.so

LoadModule setenvif_module modules/mod_setenvif.so

#LoadModule slotmem_plain_module modules/mod_slotmem_plain.so

#LoadModule slotmem_shm_module modules/mod_slotmem_shm.so

#LoadModule socache_dbm_module modules/mod_socache_dbm.so

#LoadModule socache_memcache_module modules/mod_socache_memcache.so

LoadModule socache_shmcb_module modules/mod_socache_shmcb.so

#LoadModule speling_module modules/mod_speling.so

LoadModule ssl_module modules/mod_ssl.so

LoadModule status_module modules/mod_status.so

#LoadModule substitute_module modules/mod_substitute.so

#LoadModule unique_id_module modules/mod_unique_id.so

#LoadModule userdir_module modules/mod_userdir.so

#LoadModule usertrack_module modules/mod_usertrack.so

#LoadModule version_module modules/mod_version.so

#LoadModule vhost_alias_module modules/mod_vhost_alias.so

#LoadModule watchdog_module modules/mod_watchdog.so

#LoadModule xml2enc_module modules/mod_xml2enc.so

```
##mod jk configuration version 1

```code
LoadModule jk_module modules/mod_jk.so

JkWorkersFile conf/workers.properties

JkLogLevel 		error

JkLogFile 		logs/mod_jk.log

JkMount 		/HelloWorld/* lb

<Location /jkmanager/>

	JkMount jkstatus

	Order deny,allow
    
	Deny from all
    
	Allow from 127.0.0.1
    
</Location>
```

