Oracle estimate user data size:

    select sum(bytes)/1024/1024 as size_mb, segment_type from user_segments group by segment_type;
