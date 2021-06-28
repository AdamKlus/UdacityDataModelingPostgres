# Sparkify Database

Database have 2 sources (JSON): log_data and song_data. 

ETL is processing both source files into star schema database optimised for queries on song play analysis

Fact Table
1. songplays - records in log data associated with song plays i.e. records with page NextSong
songplay_id, start_time, user_id, level, song_id, artist_id, session_id, location, user_agent
Dimension Tables
2. users - users in the app
user_id, first_name, last_name, gender, level
3. songs - songs in music database
song_id, title, artist_id, year, duration
4. artists - artists in music database
artist_id, name, location, latitude, longitude
5. time - timestamps of records in songplays broken down into specific units
start_time, hour, day, week, month, year, weekday

To run the code locally Ive used https://github.com/kenhanscombe/project-postgres/blob/master/create-docker-image.md
