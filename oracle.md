Oracle estimate user data size:

    select sum(bytes)/1024/1024 as size_mb, segment_type from user_segments group by segment_type;


## References

What to index
http://docs.oracle.com/cd/B28359_01/server.111/b28274/data_acc.htm#PFGRF004
