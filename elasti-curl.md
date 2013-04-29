Endpoint

    http://localhost:9200/_all//_search

Simplest query string search

    {
        "query" : {
        "query_string" : { 
          "query" :"your query string with \"escaped double\" quote"
        }
      }
    }

Page + Sort query

    {
        "from" : 0, "size" : 10,
        "sort" : [
          { "post_date" : {"order" : "asc"} },
          "user",
          { "name" : "desc" },
          { "age" : "desc" },
          "_score"
        ],
        "query" : {
        "query_string" : { 
          "query" :"your query string with \"escaped double\" quote"
        }
      }
    }    
