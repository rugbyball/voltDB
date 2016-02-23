schema.xml
===

<pre><code>
<uniqueKey>id</uniqueKey>  

<field name="id" type="string" indexed="true" stored="true" required="true" multiValued="false" />  

<field name="id" type="string" indexed="true" stored="true" required="false" multiValued="false" />   

</code></pre>

solrconfig.xml
===
<pre><code>
<searchComponent name="elevator" class="solr.QueryElevationComponent" >  
    <str name="queryFieldType">string</str>  
    <str name="config-file">elevate.xml</str>  
</searchComponent>  
</code></pre>

