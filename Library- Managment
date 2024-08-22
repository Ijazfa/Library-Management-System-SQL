create database Librarymanagement;
use Librarymanagement;

-- create book table
create table Books (
Book_id int primary key Auto_increment,
Title varchar(225),
Author varchar(225),
Gener varchar(225),
Published_year year,
Avilable_copies int
);
alter table Books change Avilable_copies Available_copies int;
alter table Books change Gener Genre varchar(225);

-- create members table
create table Members (
Member_id int primary key auto_increment,
Name Varchar(225),
Contact_info varchar(225),
Membership_date date
);

-- create loan table
create table Loan (
Loan_id int primary key auto_increment,
Book_id int,
Member_id int,
Loan_data date,
Return_data date,
foreign key (Book_id) references Books(Book_id),
foreign key (Member_id) references Members(Member_id)
);
alter table Loan change Loan_data Loan_date date;
alter table Loan change Return_data Return_date date;

-- create fines table 
create table Fines (
Fines_id int primary key auto_increment,
Member_id int,
Amount decimal (10,2),
Fine_date date,
Paid_status boolean,
foreign key (Member_id) references Members(Member_id)
);

alter table Books modify Published_year varchar(10);

-- sample book data

insert into Books (Title, Author, Gener, Published_year, Avilable_copies)
VALUES
('The Catcher in the Rye', 'J.D. Salinger', 'Fiction', 1951, 5),
('To Kill a Mockingbird', 'Harper Lee', 'Fiction', 1960, 2),
('1984', 'George Orwell', 'Dystopian', 1949, 3),
('The Great Gatsby', 'F. Scott Fitzgerald', 'Fiction', 1925, 4),
('Pride and Prejudice', 'Jane Austen', 'Romance', 1813, 7),
('Moby Dick', 'Herman Melville', 'Adventure', 1851, 3),
('War and Peace', 'Leo Tolstoy', 'Historical Fiction', 1869, 6),
('The Odyssey', 'Homer', 'Epic', -800, 8),
('Hamlet', 'William Shakespeare', 'Drama', 1600, 4),
('The Hobbit', 'J.R.R. Tolkien', 'Fantasy', 1937, 9),
('Ulysses', 'James Joyce', 'Modernist', 1922, 2),
('The Divine Comedy', 'Dante Alighieri', 'Epic Poetry', 1320, 5),
('Madame Bovary', 'Gustave Flaubert', 'Realism', 1857, 4),
('The Brothers Karamazov', 'Fyodor Dostoevsky', 'Philosophical Fiction', 1880, 3),
('Crime and Punishment', 'Fyodor Dostoevsky', 'Psychological Fiction', 1866, 5),
('Brave New World', 'Aldous Huxley', 'Dystopian', 1932, 6),
('Jane Eyre', 'Charlotte Bronte', 'Gothic Fiction', 1847, 7),
('Wuthering Heights', 'Emily Bronte', 'Tragedy', 1847, 4),
('Frankenstein', 'Mary Shelley', 'Gothic Fiction', 1818, 5),
('The Picture of Dorian Gray', 'Oscar Wilde', 'Philosophical Fiction', 1890, 4),
('Anna Karenina', 'Leo Tolstoy', 'Romance', 1877, 3),
('The Iliad', 'Homer', 'Epic', -760, 7),
('Don Quixote', 'Miguel de Cervantes', 'Adventure', 1605, 4),
('One Hundred Years of Solitude', 'Gabriel Garcia Marquez', 'Magical Realism', 1967, 6),
('In Search of Lost Time', 'Marcel Proust', 'Modernist', 1913, 2),
('The Trial', 'Franz Kafka', 'Absurdist Fiction', 1925, 3),
('Les Miserables', 'Victor Hugo', 'Historical Fiction', 1862, 5),
('Dracula', 'Bram Stoker', 'Horror', 1897, 4),
('Fahrenheit 451', 'Ray Bradbury', 'Dystopian', 1953, 8),
('The Stranger', 'Albert Camus', 'Philosophical Fiction', 1942, 6),
('The Count of Monte Cristo', 'Alexandre Dumas', 'Adventure', 1844, 9); 

-- sample members data
INSERT INTO Members (Name, Contact_Info, Membership_Date)
VALUES
('Alice Johnson', 'alice@example.com', '2023-01-10'),
('Bob Smith', 'bob@example.com', '2023-02-15'),
('Charlie Brown', 'charlie@example.com', '2023-03-20'),
('David Wilson', 'david@example.com', '2023-04-25'),
('Eve Davis', 'eve@example.com', '2023-05-30'),
('Frank Miller', 'frank@example.com', '2023-06-14'),
('Grace Lee', 'grace@example.com', '2023-07-18'),
('Henry Clark', 'henry@example.com', '2023-08-22'),
('Irene Turner', 'irene@example.com', '2023-09-05'),
('Jack Harris', 'jack@example.com', '2023-10-10'),
('Karen Walker', 'karen@example.com', '2023-11-14'),
('Liam King', 'liam@example.com', '2023-12-19'),
('Mia Young', 'mia@example.com', '2024-01-23'),
('Noah Allen', 'noah@example.com', '2024-02-27'),
('Olivia Scott', 'olivia@example.com', '2024-03-30'),
('Paul Martinez', 'paul@example.com', '2024-04-02'),
('Quincy Lopez', 'quincy@example.com', '2024-05-15'),
('Rachel Green', 'rachel@example.com', '2024-06-20'),
('Samuel Adams', 'samuel@example.com', '2024-07-25'),
('Tina Brooks', 'tina@example.com', '2024-08-30'),
('Uma Thurman', 'uma@example.com', '2024-09-04'),
('Victor Hugo', 'victor@example.com', '2024-10-09'),
('Wendy Peters', 'wendy@example.com', '2024-11-14'),
('Xander Harris', 'xander@example.com', '2024-12-19'),
('Yvonne Strahovski', 'yvonne@example.com', '2025-01-23'),
('Zachary Quinto', 'zachary@example.com', '2025-02-27');

-- sample loan data

INSERT INTO Loan (Book_ID, Member_ID, Loan_Date, Return_Date) 
VALUES 
(156, 1, '2024-08-01', '2024-08-15'), 
(157, 2, '2024-08-05', NULL), 
(158, 3, '2024-08-10', NULL), 
(159, 4, '2024-08-12', '2024-08-26'), 
(160, 5, '2024-08-13', NULL), 
(161, 6, '2024-08-14', '2024-08-28'), 
(162, 7, '2024-08-15', NULL), 
(163, 8, '2024-08-16', NULL), 
(164, 9, '2024-08-17', '2024-08-31'), 
(165, 10, '2024-08-18', NULL), 
(166, 11, '2024-08-19', '2024-09-02'), 
(167, 12, '2024-08-20', NULL), 
(168, 13, '2024-08-21', '2024-09-04'), 
(169, 14, '2024-08-22', NULL), 
(170, 15, '2024-08-23', '2024-09-06'), 
(171, 16, '2024-08-24', NULL), 
(172, 17, '2024-08-25', '2024-09-08'), 
(173, 18, '2024-08-26', NULL), 
(174, 19, '2024-08-27', '2024-09-10'), 
(175, 20, '2024-08-28', NULL), 
(176, 21, '2024-08-29', '2024-09-12'), 
(177, 22, '2024-08-30', NULL), 
(178, 23, '2024-08-31', '2024-09-14'), 
(179, 24, '2024-09-01', NULL), 
(180, 25, '2024-09-02', '2024-09-16'), 
(181, 1, '2024-09-03', NULL), 
(182, 2, '2024-09-04', '2024-09-18'), 
(183, 3, '2024-09-05', NULL), 
(184, 4, '2024-09-06', '2024-09-20'), 
(185, 5, '2024-09-07', NULL);

-- sample fine data

INSERT INTO Fines (Member_ID, Amount, Fine_Date, Paid_Status)
VALUES
(1, 50.00, '2024-08-20', FALSE),
(2, 20.00, '2024-08-22', TRUE),
(3, 35.00, '2024-08-25', FALSE),
(4, 15.00, '2024-08-27', TRUE),
(5, 45.00, '2024-08-29', FALSE),
(6, 25.00, '2024-09-01', TRUE),
(7, 30.00, '2024-09-03', FALSE),
(8, 40.00, '2024-09-05', TRUE);

select* from Books;
select * from Members;
select * from Loan;
select * from Fines;

-- samble queries
-- list all the avilable books based on genre
select Genre, Title, Available_copies from Books
where Available_copies > 0 
order by Genre;

-- list down the total number of books by Author
select Author, count(*) as Total_books from Books
group by Author;

-- Identify books that have not been borrowed in the last 6 months

select Title from Books
where Book_id not in (
select Book_id from loan
where Loan_date >= date_sub(curdate(), interval 6 month)
);

-- list of all books who have overdue

select m.Name, m.Contact_info, l.Loan_date 
from Members m 
join Loan l on m.Member_id = l.Member_id 
where l.Return_date is null and l.Loan_date < date_sub(curdate(), interval 14 day);

-- totla number of books borrowed  by each member

select m.Name, count(l.Loan_id) as total_Loan
from Members m 
join Loan l on m.Member_id = l.Member_id
group by m.Name;

-- total number of book in current loan

select count(*) as Total_Books_On_loan
from Loan
where return_date is Null;

-- dentify the most borrowed books

select b.Title, count(l.Loan_id) as time_borrowed
from Books b
join Loan l on b.Book_id = l.Book_id
group by b.Title
order by time_borrowed
limit 5;

-- Calculate the total amount of fines owed by each member

select m.Name, sum(f.Amount) as total_amount
from Members m
join Fines f on m.Member_id = f.Member_id
where f.paid_status = False
group by m.Name;

-- List all fines that have been paid and those that are outstanding

select m.Name, f.Amount, f.Fine_date, f.paid_status 
from Fines f
join Members m on f.Member_id = m.Member_id
order by f.paid_status asc, f.Fine_date desc;

