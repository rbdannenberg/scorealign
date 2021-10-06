# Note

This is a placeholder and not the final directory structure. The code here is
good, but it's a complete copy of PortMedia from SourceForge and will be
pared down to ScoreAlign in the future. -RD

# ScoreAlign

ScoreAlign aligns
audio-to-audio, audio-to-MIDI or MIDI-to-MIDI using dynamic time warping (DTW)
of a computed chromagram representation. There are some added smoothing tricks
to improve performance. This library is written in C and runs substantially 
faster than most other implementations, especially those written in MATLAB,
due to the core DTW algorithm. Users should be warned that while chromagrams
are robust features for alignment, they achieve robustness by operating at 
fairly high granularity, e.g., durations of around 100ms, which limits 
time precision. Other more recent algorithms can doubtless do better, but
be cautious of claims, since it all depends on what assumptions you can 
make about the music. 

This library and application were originally written as a new Audacity
feature, but the complexity of user interface extensions to manipulate
tempo in Audacity Note Tracks, along with much other new code was too
much to get into production. I offer the code here (and on SourceForge
in the PortMedia project for anyone.)
