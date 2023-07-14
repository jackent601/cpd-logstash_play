# logstash_play
learning logstash. This repo has some example docker-compose scripts for different logstash instantiations

## Notes
 - the /logstash/config/config.conf file doesn't seem to be needed if a pipeline is provided, what does it actually do then?

## logstash_tcp_input
Compose the docker file
In a separate terminal connect to 127.0.0.1:5044 with netcat, send messages and see them appear in running docker terminal

## file_input_logstash
Reads text files in a dummyData directory
Notes:
- In order to read files originally in directory ingore_older and start_position needed set.
- start_position only affects the first read
- ignore_older set to 1 day, hence if older than a day file will need updated. 
