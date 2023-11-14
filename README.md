## SQL-Basic-Create-Database-Table-and-Insert-

# CREATE DATABASE Students Record

# CREATE TABLE StudentsInfo
(StudentID INT Primary Key Identity (0001,1),
Gender VARCHAR(10) ,
Name VARCHAR(50),
Age INT,
Subject VARCHAR(50)
)

# INSERT INTO StudentsInfo VALUES
('Female', 'Amanda Eze', 25, 'Geography'),
('Male', 'Jamiu Moshood', 30, 'Chemistry'),
('Female', 'Joy Etuk', 22, 'Biology'),
('Female', 'Peter Samuel', 24, 'Mathematics');
**ALTER TABLE StudentsInfo DROP COLUMN Age;**

# CREATE TABLE HealthRecords
(HealthID INT Primary Key Identity (0001,1),
BloodGroup VARCHAR(5),
Height INT,
Weight INT,
)

# INSERT INTO HealthRecords VALUES
('AB', 175.24, 55),
('0', 198.22, 65),
('A', 150.12, 50),
('B', 145.20, 60);

# CREATE TABLE Performance
(StudentID INT IDENTITY (0001,1),
HealthID INT, Score INT, Grade VARCHAR(5),
FOREIGN KEY (StudentID) REFERENCES StudentsInfo(StudentID),
FOREIGN KEY (HealthID) REFERENCES HealthRecords(HealthID),
)

# INSERT INTO Performance VALUES
(0001, 98, 'A'),
(0002, 50, 'C'),
(0003, 20, 'F'),
(0004, 65, 'B');

# SELECT * FROM HealthRecords;

# SELECT * FROM Performance;

# SELECT * FROM StudentsInfo;
![SQL Basic Create Table_Insert](https://github.com/KemyMor/SQL-Basic-Create-Database-Table-and-Insert-/blob/a3bf1312c0b7a2c7f6c5b7833d39a4a1967cebea/SQL%20Basic%20Create%20Table_Insert.jpg)

