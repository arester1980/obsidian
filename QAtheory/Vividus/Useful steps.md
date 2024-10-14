**Timestamp validation**
```
When I save a JSON element from response by JSON path '$.[0]..timestamp' to STORY variable 'timestampRequestJson'  
When I initialize the STORY variable 'timestampRequest' with value '#{removeWrappingDoubleQuotes(#{replaceFirstByRegExp(\[(._)\], 1,1,1,{timestampRequestJson})})}'  
When I initialize the STORY variable 'timestampRequestFormatted' with value '#{formatDateTo("${timestampRequest}", "yyyy-MM-dd'T'HH:mm:ss.SSS'Z'", yyyy-MM-dd'T'HH:mm)}'  
When I initialize the STORY variable 'timestampRequestFormattedCut' with value '#{replaceFirstByRegExp(^(._)\d\d, 1,1,1,{timestampRequestFormatted})}'  
Then '${timestampRequestFormattedCut}' is EQUAL_TO '#{replaceFirstByRegExp(^(.*)\d\d, $1, #{generateDate(P, yyyy-MM-dd'T'HH:mm)})}'
```

**Save data to variable**  
```
When I set 'data-row-key' attribute value of the element by By.xpath((//_[contains(@class,'ant-table-row')])[1]) to the STORY variable 'CountID'
```