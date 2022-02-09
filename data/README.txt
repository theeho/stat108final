
========SONG CHARACTERISTICS========
 
Spotifys "Audio Features"
Definitions copied from https://developer.spotify.com/documentation/web-api/reference/#/operations/get-audio-features

acousticness: float
A confidence measure from 0.0 to 1.0 of whether the track is acoustic.
1.0 represents high confidence the track is acoustic.

danceability: float
Describes how suitable a track is for dancing based on
a combination of musical elements including tempo, rhythm stability,
beat strength, and overall regularity. A value of 0.0 is least
danceable and 1.0 is most danceable.

duration_ms: integer
The duration of the track in milliseconds.

energy: float
A measure from 0.0 to 1.0 and represents a perceptual
measure of intensity and activity. Typically, energetic tracks 
feel fast, loud, and noisy. For example, death metal has high
energy, while a Bach prelude scores low on the scale. Perceptual
features contributing to this attribute include dynamic range,
perceived loudness, timbre, onset rate, and general entropy.

instrumentalness: float 
Predicts whether a track contains no vocals. "Ooh" and "aah" sounds
are treated as instrumental in this context. Rap or spoken word tracks 
are clearly "vocal". The closer the instrumentalness value is to 1.0, 
the greater likelihood the track contains no vocal content. Values
above 0.5 are intended to represent instrumental tracks, but confidence 
is higher as the value approaches 1.0.

key: integer
The key the track is in. Integers map to pitches using standard 
Pitch Class notation. E.g. 0 = C, 1 = C♯/D♭, 2 = D, and so on. If no 
key was detected, the value is -1.

liveness: flaot 
Detects the presence of an audience in the recording. Higher liveness 
values represent an increased probability that the track was performed 
live. A value above 0.8 provides strong likelihood that the track is live.

loudness: float
The overall loudness of a track in decibels (dB). Loudness values are 
averaged across the entire track and are useful for comparing relative 
loudness of tracks. Loudness is the quality of a sound that is the primary 
psychological correlate of physical strength (amplitude). Values typically 
range between -60 and 0 db.

mode: integer
Indicates the modality (major or minor) of a track, the type of scale 
from which its melodic content is derived. Major is represented by 1 
and minor is 0.

speechiness: float
Detects the presence of spoken words in a track. The more 
exclusively speech-like the recording (e.g. talk show, audio book, poetry), 
the closer to 1.0 the attribute value. Values above 0.66 describe tracks 
that are probably made entirely of spoken words. Values between 0.33 and 
0.66 describe tracks that may contain both music and speech, either in 
sections or layered, including such cases as rap music. Values below 0.33 
most likely represent music and other non-speech-like tracks

tempo: float
The overall estimated tempo of a track in beats per minute (BPM). In 
musical terminology, tempo is the speed or pace of a given piece and derives 
directly from the average beat duration.

time_signature: integer
An estimated time signature. The time signature (meter) is a notational 
convention to specify how many beats are in each bar (or measure). The time 
signature ranges from 3 to 7 indicating time signatures of "3/4", to "7/4".

valence: float
A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a 
track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), 
while tracks with low valence sound more negative (e.g. sad, depressed, angry).


=====METRICS USED FOR CALCULATING RESPONSE VAR=======

release date: string
Date the song was released. Either day specific or year specific. 
Format is year-month-day if day specific. Example: "2021-10-29"
Format is just year if year specific. Example: "2019"

pop: integer
The sum of popularity of all artists on the track. Popularity is Spotify's metric
for measuring how popular an artist is currently.
From Spotify - The popularity of the artist. The value will be between 0 and 100, with 100 
being the most popular. The artist's popularity is calculated from the popularity of all the 
artist's tracks.

follow: integer
The sum of followers of all artists on the track. 

num artists: integer
How many artists made the track

track popularity: 
Spotify's metric for measuring how popular the track is currently. 
From Spotify - The popularity of a track is a value between 0 and 100, with 100 being the 
most popular. The popularity is calculated by algorithm and is based, in the most part, on the 
total number of plays the track has had and how recent those plays are. Generally speaking, 
songs that are being played a lot now will have a higher popularity than songs that were played 
a lot in the past. Duplicate tracks (e.g. the same track from a single and an album) are rated 
independently. Artist and album popularity is derived mathematically from track popularity. Note: 
the popularity value may lag actual popularity by a few days: the value is not updated in real time.



