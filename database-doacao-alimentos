CREATE DATABASE M3;

USE M3;

CREATE TABLE User (
   id_user  INT AUTO_INCREMENT PRIMARY KEY,
   name VARCHAR(100) ,
   address VARCHAR(500) ,
   phone CHAR(11) ,
   email VARCHAR(100) 
  );

CREATE TABLE Request (
  id_request INT AUTO_INCREMENT PRIMARY KEY,
  date_donation DATE,
  type_food VARCHAR(100),
  quantity INT, 
  id_user INT,
  FOREIGN KEY (id_user) REFERENCES User(id_user));


CREATE TABLE Donation (
  id_donation INT AUTO_INCREMENT PRIMARY KEY,
  date_donation DATE,
  type_food VARCHAR(100),
  quantity INT,
  id_request INT,
FOREIGN KEY (id_request) REFERENCES Request(id_request)
);

CREATE TABLE Donor (
  id_donor INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100),
  address VARCHAR(500),
  phone CHAR(11),
  email VARCHAR(100));


CREATE TABLE Donation_has_Donor (
  id_donation INT ,
  id_donor INT,
  FOREIGN KEY (id_donation)  REFERENCES Donation (id_donation),
  FOREIGN KEY (id_donor) REFERENCES Donor (id_donor)
  );
  
INSERT INTO User(name,address,phone,email) VALUES 
("Rodrigo","Av. América", "61943823247","rodrigo@gmail.com"),
("Stéphanie","Rua Canto das Árvores", "12345678987","stephanie@gmail.com"),
("Andrei","Rua Israel", "7189387455","andrei@gmail.com"),
("Hewel","Rua ibirapuera", "1189387455","paulista@gmail.com"),
("Amadeu","Rua Bélgica", "9889387455","amamentir@gmail.com"),
("Matheus","Rua Budléia", "3189387455","englisher@gmail.com");


INSERT INTO Donor(name,address,phone,email) VALUES 
("Debora","Caminho 16", "87534922341","debora@gmail.com"),
("Atacarejo","Sao Caetano", "10123345621","atacarejo@gmail.com"),
("Amigos Do Bem","Rua Nova Aurora", "7189387455","amigosdobem@gmail.com"),
("Programadores do amanhã","Rua Ipubi", "11534922341","pda@gmail.com"),
("Bea","Praça João Lessa", "11123345621","bea@gmail.com"),
("Dan","Rua Maenca", "2189387455","danmilgrau@gmail.com");


INSERT INTO Request(date_donation,type_food,quantity, id_user) VALUES 
("2024-03-17", "Macarrão",10,1),
("2024-03-25", "Macarrão",10,1),
("2023-05-18","Arroz", 5,2),
("2024-06-21", "Milho",20,3),
("2024-06-22", "Milho",20,3),
("2024-06-25", "Milho",20,3),
("2024-06-30", "Milho",20,3),
("2024-07-02", "Milho",20,3),
("2024-04-17", "carne",5,4),
("2024-04-25", "carne",3,4),
("2023-04-18","carne", 10,4),
("2024-01-05", "feijão",7,5),
("2024-01-01", "feijão",3,5),
("2024-01-02","feijão", 6,5),
("2023-01-03","feijão", 20,5),
("2024-02-17", "ervilha",5,6),
("2024-02-25", "ervilha",3,6),
("2024-08-17", "ervilha",10,6),
("2024-08-25", "ervilha",20,6),
("2024-09-01", "feijão",3,5),
("2024-09-02","feijão", 6,5),
("2024-09-03","feijão", 20,5),
("2024-09-01", "feijão",3,5),
("2024-09-02","feijão", 6,5),
("2024-09-03","feijão", 20,5),
("2024-09-01", "feijão",3,5),
("2024-10-02","açucar", 6,5),
("2024-10-03","açucar", 20,3),
("2024-11-02","açucar", 6,3),
("2024-11-03","açucar", 20,3),
("2024-12-03","açucar", 20,1);

 
INSERT INTO Donation(date_donation,type_food,quantity,id_request) VALUES 
("2024-03-17", "Macarrão",10,1),
("2024-03-25", "Macarrão",10,2),
("2023-05-18","Arroz", 5,3),
("2024-06-21", "Milho",20,4),
("2024-06-22", "Milho",20,5),
("2024-06-25", "Milho",20,6),
("2024-06-30", "Milho",20,7),
("2024-07-02", "Milho",20,8),
("2024-04-17", "carne",5,9),
("2024-04-25", "carne",3,10),
("2023-04-18","carne", 10,11),
("2024-01-05", "feijão",7,12),
("2024-01-01", "feijão",3,13),
("2024-01-02","feijão", 6,14),
("2023-01-03","feijão", 20,15),
("2024-02-17", "ervilha",5,16),
("2024-02-25", "ervilha",3,17),
("2024-08-17", "ervilha",10,18),
("2024-08-25", "ervilha",20,19),
("2024-09-01", "feijão",3,20),
("2024-09-02","feijão", 6,21),
("2024-09-03","feijão", 20,22),
("2024-09-01", "feijão",3,23),
("2024-09-02","feijão", 6,24),
("2024-09-03","feijão", 20,25),
("2024-09-01", "feijão",3,26),
("2024-10-02","açucar", 6,27),
("2024-10-03","açucar", 20,28),
("2024-11-02","açucar", 6,29),
("2024-11-03","açucar", 20,30),
("2024-12-03","açucar", 20,31);

INSERT INTO Donation_has_Donor (id_donation,id_donor) VALUES 
(1,1),
(2,1),
(3,1),
(4,1),
(5,2),
(6,2),
(7,2),
(8,3),
(9,3),
(10,3),
(11,4),
(12,4),
(13,5),
(14,5),
(15,5),
(16,6),
(17,6),
(18,1),
(19,1),
(20,1),
(21,1),
(22,2),
(23,2),
(24,2),
(25,3),
(26,3),
(27,3),
(28,6),
(29,6),
(30,5),
(31,5);


-- quantidade total de doações por mês
SELECT DATE_FORMAT(date_donation, '%Y-%m') AS month, 
COUNT(*) AS totalDonations 
FROM Donation 
GROUP BY month
ORDER BY month ASC;


-- quantidade total de pedidos por mês
SELECT DATE_FORMAT(date_donation, '%Y-%m') AS month, 
COUNT(*) AS totalRequest 
FROM Request 
GROUP BY month
ORDER BY month ASC;


-- quantidade total de alimentos doados por tipo
SELECT type_food, SUM(quantity) AS TotalQuantity
FROM Donation
GROUP BY type_food;


-- tipos de alimentos mais solicitados
SELECT type_food, COUNT(*) AS Total
FROM Request
GROUP BY type_food
ORDER BY Total DESC
LIMIT 3;

-- tipos de alimentos mais doados
SELECT type_food, COUNT(*) AS Total
FROM Donation
GROUP BY type_food
ORDER BY Total DESC
LIMIT 3;

-- quantidade de pedidos por usuario
SELECT User.name AS nome,
COUNT(Request.id_request) AS Total_Pedidos 
FROM User 
LEFT JOIN Request ON User.id_user = Request.id_user
GROUP BY User.name;


-- Doadores que mais doaram
SELECT Donor.name, 
SUM(Donation.quantity) AS total_quantidade
FROM Donor
INNER JOIN Donation_has_Donor ON Donor.id_donor = Donation_has_Donor.id_donor
INNER JOIN Donation ON Donation_has_Donor.id_donation = Donation.id_donation
GROUP BY Donor.name
ORDER BY total_quantidade DESC
LIMIT 3;

-- quantidade de doações por doador 
SELECT Donor.name, 
COUNT(Donation.id_donation) AS total_doacoes
FROM Donor
INNER JOIN Donation_has_Donor ON Donor.id_donor = Donation_has_Donor.id_donor
INNER JOIN Donation ON Donation_has_Donor.id_donation = Donation.id_donation
GROUP BY Donor.name
ORDER BY total_doacoes DESC;

-- Usuarios que mais solicitaram doações
SELECT User.name,
COUNT(Request.id_request) AS total_pedidos
FROM User
LEFT JOIN Request ON User.id_user = Request.id_user
GROUP BY User.name
ORDER BY total_pedidos DESC
LIMIT 3;

-- Média de doações por usuário
SELECT User.name,
AVG(Donation.quantity) AS media_doacoes
FROM User
LEFT JOIN Request ON User.id_user = Request.id_user
LEFT JOIN Donation ON Request.id_request = Donation.id_request
GROUP BY User.name
ORDER BY media_doacoes DESC;


-- quantidade de doacoes por ano
SELECT YEAR(date_donation) AS ano,
COUNT(*) AS total_doacoes
FROM Donation
GROUP BY ano
ORDER BY ano;


-- Média de Doações por Tipo de Alimento
SELECT type_food, AVG(quantity) AS MediaDoacoes
FROM Donation
GROUP BY type_food;

