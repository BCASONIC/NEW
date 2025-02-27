CREATE TABLE Students (
    RollNo VARCHAR(10) PRIMARY KEY,
    Name VARCHAR(50),
    HostelRoomNo INT,
    cgpa DECIMAL(3, 2)
);
INSERT INTO Students (RollNo, Name, HostelRoomNo, cgpa) VALUES
('99305017', 'Sai Sundar', 101, 7.23),
('99305018', 'Shyam Sundar', 111, 9.23),
('99305019', 'Ram Sundar', 112, 8.32),
('99305020', 'Priya Sharma', 103, 8.45),
('99305021', 'Anjali Singh', 104, 9.10);
SELECT * FROM Students;
SELECT RollNo FROM Students;
SELECT RollNo, Name FROM Students WHERE cgpa > 9.00;
UPDATE Students SET cgpa = 9.46 WHERE RollNo = '99305018';
DELETE FROM Students WHERE RollNo = '99305018';
