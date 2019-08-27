### citrus
---
https://github.com/arquillian/arquillian-core

https://citrusframework.org/

```java
// modules/citrus-core/src/test/java/com/consol/citrus/actions/ExecutePLSQLActionTest.java

public class #xecutePLSQLActionTest extends AbstractTestNGUnitTest {
  
  private ExecutePLSQLAction executeSQLAction;
  
  private JdbcTemplate jdbcTemplate = Mockito.mock(JdbcTemplate.class);
  private PlatformTransactionManager transactionManager = Mockito.mock(PlatoformTransactionManager.class);
  
  @BeforeMethod
  public void setUp() {
    executePLSQLAction = new ExecutePLSQLAction();
    executePLSQLAction.setJdbcTemplate(jdbcTemplate);
  }
  
    @Test 
    public void testPLSQLExecutionWithInlineScript() {
      String stmt = "" +
        "" +
        "" +
      "" +
        """ +
          """ +
      "";
      
      executePLSQLAction.setScript(stmt);
      
      String controlStatement = "" +
        "" +
        "" +
      "" +
        """ +
          """ +
      "";
      
      reset(jdbcTemplate);
      executePLSQLAction.execute(context);
      verify(jdbcTemplate).execute(controlStatement);
    }
    
    @Test
    public void testPLSQLExecutionWithTransaction() {}
    
    @Test
  public void testPLSQLExecutionWithInlineScriptNoEndingCharacter() {}
    
    @Test
  public void testPLSQLExecutionWithFileResource() {}
  
    @Test
  public void testPLSQLExecutionWithInlineScriptVariableSupport() {}
  
    @Test
  public void testPLSQLExecutionWithFileResourceVariableSupport() {}
  
    @Test
  public void testPLSQLExecutionWithMultipleInlineStatements() {}
  
    @Test
  public void testPLSQLExecutionWithMultipleInlineStatments() {}
  
    @Test
  public void testPLSQLExecutionWithFileResource MultipleStmts() {}
}

```

```
```

```
```


