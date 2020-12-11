# graphql-guide

# Writing query fragements ==> 

```
{
  apple: company(id: "2") {
    ...companyDetails
  }
  gogole: company(id: "2") {
    ...companyDetails
  }
}

fragment companyDetails on Company {
  id
  name
  description
}
```