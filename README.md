Munin Solr plugin
=================

Munin wildcard plugin to monitor Apache Solr cores. This plugin uses XML::XPath
to extract statistics from the `stats.jsp` page in the Apache Solr web interface.

The current version of the plugin has been tested with Solr 3.6.x.


Configuration
-------------

This plugin has the following default settings (for a Solr core available at `http://127.0.0.1:8983/solr/`):

    [solr_core0_*]
        env.scheme http
        env.host 127.0.0.1
        env.port 8983
        env.path solr
        env.query_handler /select

You can override the defaults by placing a configuration file in the
plugin-conf.d directory.
