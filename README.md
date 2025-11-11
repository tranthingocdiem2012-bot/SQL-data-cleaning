# SQL-data-cleaning
SQL data cleaning
SELECT* from club_member_info cmi
limit 10;
select* from club_member_info cmi;
CREATE TABLE club_member_info_cleaned (
	full_name VARCHAR(50),
	age INTEGER,
	martial_status VARCHAR(50),
	email VARCHAR(50),
	phone VARCHAR(50),
	full_address VARCHAR(50),
	job_title VARCHAR(50),
	membership_date VARCHAR(50)
);
INSERT INTO  club_member_info_cleaned
Select*from club_member_info;
UPDATE club_member_info_cleaned
set full_name =trim(full_name )

UPDATE club_member_info_cleaned
set full_name= UPPER(full_name )
