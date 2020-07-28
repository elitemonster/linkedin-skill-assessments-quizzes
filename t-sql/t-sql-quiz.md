## T-SQL Assessment


#### Q1. Which answer is NOT a type of table index?

- [ ] nonclustered
- [x] unique
- [ ] heap
- [ ] hash

#### Q2. The keywords AND, IN, LIKE, and between all belong to a category called what? 

- [ ] joining operations
- [x] linking operations
- [ ] criteria operations
- [ ] logical operations

#### Q3. What is the result of this series of statements?

BEGIN TRY
    SELECT 'Foo' AS Result;
END TRY
BEGIN CATCH
 SELECT 'Bar' AS Result;
END CATCH

- [x] Foo
- [ ] FooBar
- [ ] Foo Bar
- [ ] Bar

#### Q4. Given these two tables, which query generates a listing showing student names and the department office location where you could reach each student? 

- [ ] SELECT Students.first_name, Students.last_name, Departments.office_location FROM Students, Departments;
- [x] SELECT Students.first_name, Students.last_name, Departments.office_location FROM Students ON Students JOIN Departments ON Students.department = Departments.department;
- [ ] SELECT Students.first_name, Students.last_name, Departments.office_location FROM Students JOIN Departments;
- [ ] SELECT Students.first_name, Students.last_name, Departments.office_location FROM Students ON Students.department = Departments.department;

#### Q5. What is an example of a DDL command in SQL?

- [ ] TRUNCATE TABLE
- [ ] DELETE
- [ ] MERGE
- [x] DROP

#### Q6. Given the Games table pictured, which query generates the results shown?

- [ ] SELECT GameType, MaxPlayers, count(*) AS NumberOfGames
      FROM Games
      GROUP BY MaxPlayers, GameType
      ORDER BY MaxPlayers, GameType;
- [x] SELECT GameType, MaxPlayers, count(*) AS NumberOfGames
      FROM Games
      GROUP BY GameType, MaxPlayers
      ORDER BY GameType;
- [ ] SELECT GameType, count(Players) AS MaxPlayers, NumberOfGames
      FROM Games
      GROUP BY GameType, MaxPlayers
      ORDER BY GameType;
- [ ] SELECT GameType, MaxPlayers, count(*) AS NumberOfGames
      FROM Games
      GROUP BY GameType
      ORDER BY MaxPlayers;

#### Q7. Which answer is a possible result of the sequence of commands below?

DECLARE @UniqueID uniqueidentifier = NEWID();
SELECT @UniqueID AS Result;

- [ ] 1
- [x] bb261196-66a5-43af-815d-123fc593cf3a
- [ ] z350mpj1-62lx-40ww-9ho0-4u1875rt2mx4
- [ ] 0x2400001155F04846674AD4590F832C0

#### Q8. You need to find all students that are not on the "Chemistry Cats" team. Which query does NOT work for this task?

- [ ] SELECT * FROM Students
      WHERE team NOT 'Chemistry Cats';

- [ ] SELECT * FROM Students
      WHERE team <> 'Chemistry Cats';

- [ ] SELECT * FROM Students
      WHERE team != 'Chemistry Cats';

- [x] SELECT * FROM Students
      WHERE NOT team = 'Chemistry Cats';

#### Q9. You need to write a query that returns all Employees that have a LastName starting with the letter A. Which WHERE clause should you use to fill in the blank in this query? 

- [ ] WHERE LastName = A*
- [ ] WHERE LastName = LIKE '%A%'
- [x] WHERE LastName LIKE 'A%
- [ ] WHERE LastName IN ('A*')

#### Q10. Which query shows the first name, department, and team of all students with the two lowest points?

- [ ] SELECT LIMIT(2) first_name, department, team FROM Students ORDER BY points ASC;
- [x] SELECT TOP(2) first_name, deprtment, team FROM Students ORDER BY points DESC;
- [ ] SELECT TOP(2) WITH TIES first_name, department, team FROM Students ORDER BY points;
- [ ] SELECT BOTTOM(2) first_name, department, team FROM Students ORDER BY points ASC;

#### Q11. What is the result of this statement?

SELECT FLOOR(-1234.321)

- [ ] -1234.3
- [ ] -1234
- [x] -1235
- [ ] 1234.321

#### Q12. Which is the best approach to update the last name of the student Donette Figgins to Smith

- [x] UPDATE Students SET last_name = 'Smith' WHERE email = 'dfiggins@rouxacademy.com';
- [ ] UPDATE Students SET last_name = 'Figgins' WHERE email = 'dfiggins@rouxacademy.com';
- [ ] UPDATE Students SET last_name = 'Figgins' WHERE last_name = 'Smith' AND first-name = 'Donette';
- [ ] UPDATE Students SET last_name = 'Smith' WHERE last_name = 'Figgins' AND first-name = 'Donette';

#### Q13. Which of these data types is an approximate numeric?

- [x] real
- [ ] bit
- [ ] decimal
- [ ] numeric

#### Q14. You need to remove all data from a table name Products. Which query fully logs the removal of each record?

- [ ] TRUNCATE FROM Products *;
- [x] DELETE FROM Products;
- [ ] DELETE * FROM Products;
- [ ] TRUNCATE TABLE Products;  

#### Q15. What is the result of the following query? SELECT 1 / 2 AS Result;

- [ ] 0.5
- [ ] error
- [x] 0
- [ ] 2

#### Q16. which data type will most efficiently store a person's age in years?

- [ ] float
- [ ] int
- [x] tinyint
- [ ] bigint

#### Q17. What is the result of this query?

SELECT 'abc\
def' AS Result;

- [ ] abc\def
- [x] abcdef
- [ ] error
- [ ] abc def

#### Q18. To select a random student from the table, which statement could you use?

- [x] SELECT TOP(1) first_name, last_name FROM Students ORDER BY NEWID();
- [ ] SELECT TOP(1) RAND(first_name, last_name) FROM Student;
- [ ] SELECT TOP(1) first_name, last_name FROM Student;
- [ ] SELECT TOP(1) first_name, last_name FROM RAND(Student);

#### Q19. What result is returned after executing the following commands?

    DECLARE @MyVariable int;
    SET @MyVariable = 1;
    GO 
    SELECT @MyVariable;

- [x] error
- [ ] 1
- [ ] null
- [ ] @MyVariable

#### Q20. Which statement creates a new database schema named Sales and establish Sharon as the owner?

- [ ] ALTER USER Sharon WITH DEFAULT_SCHEMA = Sales;
- [ ] ALTER USER Sharon SET SCHEMA Sales;
- [x] CREATE SCHEMA Sales SET OWNER Sharon;
- [ ] CREATE SCHEMA Sales AUTHORIZATION Sharon;

#### Q21. The result of a CROSS JOIN between a table with 4 rows, and one with 5 rows, will give with ____ rows.

- [ ] 1024
- [x] 20
- [ ] 0
- [ ] 9