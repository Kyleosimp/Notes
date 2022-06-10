create database classwork;

show databases;

use classwork;

show tables;

create table movies(title text, runtime integer, genre text, imdb_score float, rating text);

insert into movies (title, runtime, genre, imdb_score, rating)
values ('Howard the Duck',110,'Sci-Fi',4.6,'PG');

insert into movies (title, runtime, genre, imdb_score, rating)
values ('Lavantula',83,'Horror',4.7,'TV-14');

insert into movies (title, runtime, genre, imdb_score, rating)
values ('Starship Troopers',129,'Sci-Fi',4.6,'PG-13');

insert into movies (title, runtime, genre, imdb_score, rating)
values ('Waltz with Bashir',129,'Sci-Fi',7.2,'PG-13');

insert into movies (title, runtime, genre, imdb_score, rating)
values ('Spaceballs',96,'Comedy',7.1,'PG');

insert into movies (title, runtime, genre, imdb_score, rating)
values ('Monsters Inc.',92,'Animation',8.1,'G');

select from * movies;

insert into movies (title, runtime, genre, imdb_score, rating)
values ('Spider-Man No Way Home',148,'Action',8.3,'PG-13');

insert into movies (title, runtime, genre, imdb_score, rating)
values ('finch',115,'Adventure',6.8,'PG-13');

insert into movies (title, runtime, genre, imdb_score, rating)
values ('Code 8',98,'Thriller',6.1,'Not Rated');

select title, genre FROM movies where genre = 'Sci-Fi';

select title, imdb_score from movies where imdb_score>6.5;

select * FROM movies WHERE Rating = 'G' OR Rating = 'PG' -> AND Runtime <=100;

select title, avg)runtime_ from movies where imdb_score <=7.5
group by genre;

update movies set rating = 'R' where title = 'Starship Troopers';
select * from movies;

alter tables movies
add column movie_id int first;

update movies set movie_ID = 1 where title = 'Howard the Duck';
update movies set movie_ID = 2 where title = 'Lavantula';
update movies set movie_ID = 3 where title = 'Starship Troopers';
update movies set movie_ID = 4 where title = 'Waltz with Bashir';
update movies set movie_ID = 5 where title = 'Spaceballs';
update movies set movie_ID = 6 where title = 'Monsters Inc.';
update movies set movie_ID = 7 where title = 'Spider-Man No Way Home';
update movies set movie_ID = 8 where title = 'finch';
update movies set movie_ID = 9 where title = 'Code 8';

select movie_ID, title, rating from movies where genre in('Horror', 'Documentary');

select rating, avg(imdb_score),max(imdb_score),min(imdb_score) from movies group by rating;

select rating, avg(imdb_score),max(imdb_score),min(imdb_score) from movies group by rating having count(*) > 1;











