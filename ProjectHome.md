MOOV Relocator is a well documented small library written in PHP to relocate (or move) the MOOV-Atom of MP4-Files from the end to the beginning of a file.

In H.264-based video formats (mp4, m4v) the metadata is called a "moov atom". The moov atom is a part of the file that holds the index information for the whole file.

Many encoding software programs such as FFmpeg will insert this moov atom information at the end of the video file. This is bad. The moov atom needs to be located at the beginning of the file, or else the entire file will have to be downloaded before it begins playing.

Running your video file through this application makes your MP4 files ready for pseudostreaming. Of course you need to have those keyframes in place.

If you just want the source then you should checkout the current trunk from SVN. If you need the demonstration-files (_demo/demo.mp4 +_demo/index.php) then you should download the archive-release (featured download).