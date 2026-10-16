# tf2-fastdl

FastDL content for the dima TF2 server, served by GitHub Pages.

Layout mirrors `tf/`, so a map at `tf/maps/<name>.bsp` on the server lives
here at `maps/<name>.bsp.bz2`. Source clients request the `.bz2` first and
fall back to the uncompressed file, so only the compressed copy is needed.

Server side:

    sv_downloadurl "https://esqa.github.io/tf2-fastdl"
    sv_allowdownload 1
