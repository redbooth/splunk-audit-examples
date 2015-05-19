###Step 1:

####Configure Splunk Properties For Proper AeroFS Audit Data Extraction
  
If you haven't installed Splunk yet, you should do so now:
http://www.splunk.com/en_us/download/splunk-enterprise.html

1. Copy the **aerofs-props.conf** file into the `$SPLUNK_HOME/etc/system/local` directory and rename it to **props.conf**. If there is alreay a "props.conf" file in this directory, add the contents of the "aerofs-props.conf" file into the existing "props.conf" file. 

	_Depending on the operating system, the `$SPLUNK_HOME` directory will vary._ 

	Linux: 
	`$SPLUNK_HOME = /opt/splunk` 

	Mac: 
	`$SPLUNK_HOME = /Applications/Splunk/`

	Windows: `$SPLUNK_HOME = C:\Program Files\Splunk` 


2. Restart Splunk 

3. Configure the Data Input in Splunk for your AeroFS Appliance's Audit Data. More information on this here: <link_to_audit_article> 
 


###Step 2: 

#### Import Search Queries

1.  Copy the **aerofs-savedsearches.conf** file into the `$SPLUNK_HOME/etc/users/admin/search/	local` directory and rename it to **savedsearches.conf**. If there is already a 	"savedsearches.conf" file in this directory, add the contents of the "aerofs-	savedsearches.conf" into the existing "savedsearches.conf" file.

2.  Restart Splunk

3.  Log into the Splunk Web interface and from **Search and Reporting**, click on **Reports** to 	view the list of sample AeroFS Audit queries/reports. Simply click on a saved report to run 	it. 

