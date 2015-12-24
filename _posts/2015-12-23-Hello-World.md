---
layout: post
title: You're up and running! Go ahead and test it. 
---

Next you can update your site name, avatar and other options using the _config.yml file in the root of your repository (shown below).

<!-- ![_config.yml]({{ site.baseurl }}/images/config.png) -->
![_config.yml]({{ site.baseurl }}/images/config.png)

<!-- https://guides.github.com/features/mastering-markdown/  --> 


# This is an <h1> tag
## This is an <h2> tag
###### This is an <h6> tag


```
if (isAwesome){
  return true
}
```

Welcome to the myblog wiki!
# henry4sfdc_backup
henry4sfdc backup
Welcome to the henry4sfdc_backup wiki!

# Tools 
* FuseIT SFDC Explorer
* Workbench
* Mavensmate
* Eclipse Force.com IDE
* Ant
* CodeFusion IDE
* SoqlXplorer 


# JSON Parser & Generator sample
Use JSON.Generator to generate JSON string
Use JSON.Parser to parse thru JSON string (e.g. to extract property value)
Serializes Apex objects into JSON content (Object to JSON)
Deserializes the specified JSON string into an Apex object (JSON -> Object)

https://developer.salesforce.com/page/Getting_Started_with_Apex_JSON
https://developer.salesforce.com/docs/atlas.en-us.apexcode.meta/apexcode/apex_json_jsonparser.htm
http://opfocus.com/blog/json-deserialization-techniques-in-salesforce/

## Terminology - 
1. JSON object has property (e.g. Customers, Count)
1. the value of the Customer property is an array (denoted by [])
1. the value of the Count is a number
1. the array contains 3 child JSON objects; the 1st and 2nd child JSON objects have a similar structure, each containing properties that have string values.
1. Each propertiy is represented by a name:value pair
1. Properties are separated by commans. There is no common after the last property in a JSON object.  

https://scotthung.wordpress.com/2015/01/21/how-to-parse-a-json-response-using-salesforces-jsonparser-class/
In the JSON response, every character except the colon (:) is a token – unless it’s encapsulated in double quotes (“). Within double quotes, the entire string is the token.  So, many parsing routines traverse the JSON response with while (parser.nextToken() != null). 

Secondly, getCurrentToken() returns type JSONToken enum (https://developer.salesforce.com/docs/atlas.en-us.apexcode.meta/apexcode/apex_enum_System_JsonToken.htm) and getText() method returns the character(s) of that token.  So the calling getCurrentToken() at the very start of the JSON above returns START_OBJECT and getText() returns “{”. 

Thirdly, from the documentation we know:
{ and } are identified by the tokens START_OBJECT and END_OBJECT, respectively
[ and ] are identified by the tokens START_ARRAY and END_ARRAY, respectively

I’ll also add FIELD_NAME is the token on the left side of a colon and the token to the right of a colon is VALUE_xx (e.g. VALUE_STRING, VALUE_TRUE, VALUE_NULL, etc). “countryCode”:”PL”

Calling getCurrentToken() returns FIELD_NAME and getText() returns countryCode.  If nextToken() is called then getCurrentToken() returns VALUE_STRING and getText() returns PL

Thirdly, from the documentation we know:

{ and } are identified by the tokens START_OBJECT and END_OBJECT, respectively
[ and ] are identified by the tokens START_ARRAY and END_ARRAY, respectively

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub.
