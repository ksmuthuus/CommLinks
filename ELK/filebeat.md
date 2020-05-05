[Net.ServicePointManager]::SecurityProtocol = "tls12, tls11, tls"
Invoke-WebRequest https://artifacts.elastic.co/downloads/beats/filebeat/filebeat-7.6.2-windows-x86_64.zip -OutFile 'Filebeat.zip'