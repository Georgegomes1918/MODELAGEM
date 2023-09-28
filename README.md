# MODELAGEM
## MODELAGEM CONCEITUAL 
<img width="544" alt="image" src="https://github.com/Georgegomes1918/MODELAGEM/assets/142853919/8a5cd3b2-2ad5-4cc4-ba7c-9e9f200a13e9">

## MODELAGEM LÓGICA
<img width="617" alt="image" src="https://github.com/Georgegomes1918/MODELAGEM/assets/142853919/f753852f-64b7-4835-a1c6-7073acee3f1a">

'''SQL
CREATE TABLE Alunos 
( 
 Codigo_aluno VARCHAR(10) PRIMARY KEY,  
 email VARCHAR(50) NOT NULL,  
 whatsapp INT NOT NULL,  
 idSede INT,  
 Curso VARCHAR(80) NOT NULL,  
 Nome_aluno VARCHAR(80) NOT NULL  
);


CREATE TABLE Sede 
( 
 codigo_sede INT PRIMARY KEY
 nome_sede VARCHAR(80) NOT NULL,
 Endereco VARCHAR(80) NOT NULL  
); 


ALTER TABLE Alunos ADD FOREIGN KEY(idSede) REFERENCES Alunos (idSede)

--Consultando tabelas
SELECT * FROM Alunos


SELECT * FROM sede;

--Inserindo dados
--sede
INSERT INTO sede (codigo_sede, nome_sede, endereco) VALUES (1, 'DC SUL','AV. WS...');
INSERT INTO sede (codigo_sede, nome_sede, endereco) VALUES (2, 'DC Aldeota','Av. SD...');

--alunos
INSERT INTO alunos VALUES (1, 'aaaa','a@fjfj','DA Analytics','3333333',1);

INSERT INTO alunos VALUES (2, 'bbbb','a@fjfj','DA Analytics','3333333',2),
						  (3, 'Aluno 4','a@fjfj','DA Analytics','3333333',1),
					      (5, 'Aluno 5','a@fjfj','DA Analytics','3333333',2),
						  (4, 'Aluno 6','a@fjfj','Marketing','3333333',2);
        '''

