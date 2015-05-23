# Splunk Audit Examples

This repository contains some example Splunk queries that can be used to
extract useful information from the AeroFS Private Cloud audit stream.

## Installation

1. Copy the `aerofs-props.conf` file into `$SPLUNK_HOME/etc/system/local` and
   rename it to `props.conf`. If there is alreay a `props.conf` file in this
   directory, add the contents of the `aerofs-props.conf` file into the
   existing `props.conf`.

3. Configure the Data Input in Splunk for your AeroFS Appliance's Audit Data.
   More information can be found in the
   [AeroFS Help Center Documentation](https://support.aerofs.com/hc/en-us/articles/204862650).

4. Copy the `aerofs-savedsearches.conf` file into
  `$SPLUNK_HOME/etc/users/admin/search/local` and rename it to
  `savedsearches.conf`. If there is already a `savedsearches.conf` file in this
  directory, add the contents of the `aerofs-savedsearches.conf` file into the
  existing `savedsearches.conf`.

2. Restart Splunk.

3. Log into the Splunk Web interface and from **Search and Reporting**, click
   on **Reports** to view the list of sample AeroFS Audit reports.
