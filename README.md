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

# Add user mutation
```
mutation {
  addUser(firstName: "Jhon", age: 28) {
    id
    firstName
    age
  }
}
```

# delete user mutation
```
mutation {
  deleteUser(id: "1") {
    id
  }
}
```