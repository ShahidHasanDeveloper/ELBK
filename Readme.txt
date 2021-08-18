1. download filebeat and logstash  of 7.10.2 and update the attached file respectively and run both using command line.
	(i) cd C:\Users\Shahid_Hasan\JPoP\JPoP6\development\ELBK\filebeat-7.10.2-windows-x86_64
		filebeat -e -c filebeat.yml
	(ii) cd C:\Users\Shahid_Hasan\JPoP\JPoP6\development\ELBK\logstash-7.10.2-windows-x86_64\logstash-7.10.2\bin
		 logstash -f ../config/logstash-sample.conf --config.reload.automatic


2. docker-compose up 
3. Use below if issue in elastic search to come up due to memory issue.
   wsl -d docker-desktop
   sysctl -w vm.max_map_count=1073741824
   exit
