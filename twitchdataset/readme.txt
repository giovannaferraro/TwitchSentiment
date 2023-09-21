TwitchChat: A Dataset for Exploring Livestream Chat
Charles Ringer, Mihalis A. Nicolaou, James Alfred Walker
--------------------------------------------------------

Dataset Description 
-------------------
This dataset contains chat logs from Twitch.tv. A full description of the dataset can be found in the accompanying paper. Briefly, it contains 1951 pairs of files. One file, the 'document'. titled '{streamer}_{document}.csv' contains chat logs. {streamer} is an anonymised streamer name. It is consistent between documents from the same streamers. {document} if a 0 indexed count of the particular document, given that there are multiple documents for each stream. The other file, the 'metadata', is stored in the 'Meta_Data' sub-directory and is titled '{streamer}_{document}_meta.json'

Each document is data gathered from a single stream session. Each document contains a single header row followed by rows of temporally ordered messages. There are three columns, the first 'Time' details the time in seconds between the start of the document and when the message was sent. The second 'User' contains an anonymised version of the username for the user who wrote the message, anonymised in the same way as the streamers name. The third column 'Message' contains the message sent. 

The metadata is a json document which collects the following data about the stream, gathered at the start of the data gathering process:
user_view_count, user_broadcaster_type", stream_game_id, stream_type, stream_viewer_count, stream_start_date, stream_language