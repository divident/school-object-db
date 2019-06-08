## Usage

```
USER>Do ##class(UserDB.Student).Populate(10)

USER>set s1 = ##class(UserDB.Student).OpenId(1)

SET s1 = ##CLASS(UserDB.Student).OpenId(1)

USER>zwrite s1
s1=<OBJECT REFERENCE>[1@UserDB.Student]
+----------------- general information ---------------
|      oref value: 1
|      class name: UserDB.Student
|           %%OID: $lb("116","UserDB.Student")
| reference count: 2
+----------------- attribute values ------------------
|       %Concurrency = 1  <Set>
|                %id = ""
|       %seriesCount = 1
|         CardNumber = 66903
|                 Id = 112728819
|               Name = "Cannon,Yan N."
+----------------- swizzled references ---------------
|          i%%source = ""
|          r%%source = ""
|          i%Classes = ""
|       i%Classes(1) = $lb("1")
|       i%Classes(2) = $lb("1")
|       i%Classes(3) = $lb("1")
|          r%Classes = ""  <Set>
+-----------------------------------------------------

USER>Do s1.ParticipateInClasses()

Score Biology exercise 2
Score Chemistry exercise 4
Score Math exercise 3
```
