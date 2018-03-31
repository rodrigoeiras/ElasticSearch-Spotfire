# RinR is a package from TERR to send some part of the code to the Open R engine.
library(RinR)

ElasticData <- REvaluate({
  
  library(curl);
  library(jsonlite);
  
  # You can change the result size to something you need.
  result <- fromJSON("http://10.211.55.3:9200/films/_search?size=5000")
  
  # Creating a data table from the elastic search json data.  
  jsonData <- result$hits$hits$`_source`
  
})
