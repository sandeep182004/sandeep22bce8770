SHOW DATABASES;

CREATE DATABASE vit;

USE vit;

CREATE TABLE vit_vellore (
    full_name VARCHAR(100),
    reg_no VARCHAR(20) PRIMARY KEY,
    school VARCHAR(100),
    graduation_year INT
);

INSERT INTO vit_vellore (full_name, reg_no, school, graduation_year) VALUES
('Sandeep Kumar', '21CSE2001', 'School of Computer Science', 2025),
('Aarav Joshi', '21EEE2002', 'School of Electrical Engineering', 2025),
('Ishita Roy', '21MEC2003', 'School of Mechanical Engineering', 2025),
('Tanvi Gupta', '20BCE2004', 'School of Computer Science', 2024),
('Ritika Sen', '21CSE2005', 'School of Computer Science', 2025),
('Manav Singh', '21ECE2006', 'School of Electronics Engineering', 2025),
('Reyansh Patel', '20BBA2007', 'School of Business', 2024),
('Neha Bhat', '22CIV2008', 'School of Civil Engineering', 2026),
('Rhea Chakraborty', '21BIO2009', 'School of Bio Sciences', 2025);

SELECT * FROM vit_vellore;

ALTER TABLE vit_vellore ADD(phone VARCHAR(10));

DESC vit_vellore;

ALTER TABLE vit_vellore DROP COLUMN phone;

ALTER TABLE vit_vellore ADD(s_country VARCHAR(10) DEFAULT 'India');

UPDATE vit_vellore SET full_name='Nikita Anandmani' WHERE full_name='Rhea Chakraborty';
