# Neo4jAuraDB_Ex
Example datasets for practice import .csv file in Neo4j. \
Related query 
```
LOAD CSV WITH HEADERS FROM 'https://raw.githubusercontent.com/songsong0425/Neo4jAuraDB_Ex/main/LabMembers.csv' AS row
MERGE (m:Member {memberID: row.mid})
  ON CREATE SET m.Name=row.name, m.Age=row.age, m.Sex=row.sex
```
