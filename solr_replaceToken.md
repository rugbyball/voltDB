https://github.com/apache/lucene-solr/blob/3f38aba02ce37c6422875d8824ee034d42d635b9/solr/contrib/dataimporthandler/src/java/org/apache/solr/handler/dataimport/VariableResolver.java

https://github.com/apache/lucene-solr/blob/813ca77250db29116812bc949e2a466a70f969a3/solr/contrib/dataimporthandler/src/java/org/apache/solr/handler/dataimport/ContextImpl.java

https://github.com/apache/lucene-solr/blob/813ca77250db29116812bc949e2a466a70f969a3/solr/contrib/dataimporthandler/src/java/org/apache/solr/handler/dataimport/Context.java

https://github.com/apache/lucene-solr/blob/3f38aba02ce37c6422875d8824ee034d42d635b9/solr/contrib/dataimporthandler/src/test/org/apache/solr/handler/dataimport/AbstractDataImportHandlerTestCase.java

<code>
  private Resolved getResolved(String template) {
    Resolved r = cache.get(template);
    if (r == null) {
      r = new Resolved();
      Matcher m = PLACEHOLDER_PATTERN.matcher(template);
      while (m.find()) {
        String variable = m.group(1);
        r.startIndexes.add(m.start(0));
        r.endOffsets.add(m.end(0));
        r.variables.add(variable);
      }
      cache.put(template, r);
    }
    return r;
  }
</code>  
  
