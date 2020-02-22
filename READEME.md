# Guitarlian Laboratory


## Conver m4p to wav using `ffmpeg`

    1. m4p to mp3
        `ffmpeg -i c.m4a -c:a libmp3lame -ac 2 -b:a 44100 c.mp3`
        -i : input file
        -c:a encoder/decoder codec
        -ac: audio channel number
        -b:a sample rate
        
    2. mp3 to wav
        `ffmpeg -i c.mp3 -acodec pcm_u8 -ar 44100 c.wav`
        -acodec: alias for -codec:a
        -ar – Set the audio frequency of the output file. The common values used are  22050, 44100, 48000 Hz.