Parser that works with ffmpeg to read piped data and fragment mp4 into an initialization segment and media segments. It can also get the codec info and generate an fmp4 HLS m3u8 playlist. Must use the following flags with ffmpeg targeting the output: -f mp4 -movflags +faststart+frag_keyframe.

Currently being used in a media source extension project @ https://github.com/kevinGodell/mse-live-player